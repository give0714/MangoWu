---
description: Informix-4GL 資料操作_游標
---

# SCROLL CURSOR

## 一般架構

```sql
-- 宣告變數 --
DEFINE recordTableName RECORD LIKE tableName.*
-- 宣告游標 --
DECLARE cursorName CURSOR FOR
        INSERT INTO recordTableName VALUES( value1 [, value2, ...])
-- 開啟游標 --
OPEN cursorName [ USING variableName1 [, variableName2, ...]]
-- 將資料放入宣告的變數內 --
LET recordTableName.columnName = value
[...]
-- 將變數資料放入緩衝區內 --
PUT cursorName FORM recordTableName.columnName [, ...]
-- 將緩衝區的資料新增至資料表內 --
FLUSH cursorName
-- 將資料放入宣告的變數內 --
LET recordTableName.columnName = value
[...]
-- 關閉游標，並將與此游標相關的變數資料新增至資料庫內 --
CLOSE cursorName
-- 釋放游標 --
FREE cursorName
```

{% hint style="info" %}
架構：

&#x20;                <mark style="background-color:red;">PUT 指令</mark>                <mark style="background-color:red;">FLUSH 指令</mark>

程式變數        ->        入緩衝區        ->        資料庫

&#x20;                   資料                           資料
{% endhint %}

{% hint style="info" %}
流程說明：

1.  DECLARE 游標

    取得記憶體空間，以放置 CURSOR 游標，並將其指向 NULL〈指標 Point〉。
2.  OPEN 游標

    在記憶體內取得一空間，放置資料緩衝區，並將 CURSOR 的指標指向該緩衝區的起始點，但此時尚未抓取任何資料。

    將 SQL 語法傳輸到後端引擎，執行語法檢查、查詢最佳化、存取權限檢驗、暫存檔建立等作業。
3.  PUT 游標

    將欲新增之資料存入資料緩衝區內。
4.  FLUSH 游標

    將資料緩衝區內的資料，做資料驗證，並存入資料庫。
5.  CLOSE 游標

    將資料存入資料庫《不論有無存入資料緩衝區內，都會一併執行新增處理》後，關閉游標。
6.  FREE 游標

    釋放資料緩衝區的記憶體空間。
{% endhint %}



{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
