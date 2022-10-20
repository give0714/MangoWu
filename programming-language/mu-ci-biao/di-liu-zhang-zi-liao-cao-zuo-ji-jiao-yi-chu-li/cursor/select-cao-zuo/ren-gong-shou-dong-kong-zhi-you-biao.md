---
description: Informix-4GL 資料操作_游標
---

# 人工手動控制游標

## 語法

```sql
-- 宣告變數 --
DEFINE recordTableName RECORD LIKE tableName.*
-- 宣告游標 --
DECLARE cursorName CURSOR FOR
        SELECT * FROM tableName
-- 開啟游標 --
OPEN cursorName
-- 取得游標所在位置的資料庫資料 --
FLUSH [ NEXT
        / ( PREVIOUS / PRIOR )
        / FIRST
        / LAST
        / CURRENT
        / RELATIVE m
        / ABSOLUTE n ] cursorName INTO selectTableName.*
-- 關閉游標 --
CLOSE cursorName
-- 釋放游標 --
FREE cursorName
```

{% hint style="info" %}
架構：

&#x20;                       <mark style="background-color:red;">FLUSH 指令</mark>

表格        ->        輸出緩衝區        ->        程式變數

&#x20;           資料                           資料
{% endhint %}

{% hint style="info" %}
流程說明：

1.  DECLARE 游標

    取得記憶體空間，以放置 CURSOR 游標，並將其指向 NULL〈指標 Point〉。
2.  OPEN 游標

    在記憶體內取得一空間，放置資料緩衝區，並將 CURSOR 的指標指向該緩衝區的起始點，但此時尚未抓取任何資料。

    將 SQL 語法傳輸到後端引擎，執行語法檢查、查詢最佳化、存取權限檢驗、暫存檔建立等作業。
3.  FLUSH 游標

    控制游標在資料庫的位置，取得指定位置的查詢結果，並將結果寫入資料緩衝區內的記憶體空間。
4.  CLOSE 游標

    關閉游標控制。
5.  FREE 游標

    釋放資料緩衝區的記憶體空間。
{% endhint %}

{% hint style="info" %}
補充：

1.  NEXT

    控制游標往後一列。
2.  PREVIOUS

    控制游標往前一列。
3.  PRIOR

    控制游標往前一列。
4.  FIRST

    控制游標至資料第一列。
5.  LAST

    控制游標至資料最後一列。
6. CURRENT\
   控制游標到當前列。
7. RELATIVE m\
   控制游標至當前游標位置算起的第 m 列。
8. ABSOLUTE n\
   控制游標到第 n 列。
9. 除 FETCH 敘述和 FETCH NEXT 敘述外，其他均須於使用前宣告。
10. 需在 FETCH 敘述後，使用 IF 敘述來檢查狀況變數 Status 是否變更為 NOTFOUND。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
