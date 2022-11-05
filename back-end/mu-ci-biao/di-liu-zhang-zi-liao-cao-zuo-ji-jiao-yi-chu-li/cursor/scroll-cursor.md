---
description: Informix-4GL 資料操作_游標
---

# SCROLL CURSOR

## 一般架構

```sql
-- 宣告變數 --
DEFINE recordTableName RECORD LIKE tableName.*
-- 宣告游標 --
DECLARE cursorName SCROLL CURSOR [ WITH HOLD ] FOR
        SELECT *
          FROM tableName
-- 開啟游標 --
OPEN cursorName
-- 透過控制游標，來顯示緩衝區的資料表資料 --
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

## PREPARE 架構

```sql
-- 宣告變數 --
DEFINE recordTableName RECORD LIKE tableName.*
-- 宣告 SQL 語法變數 --
DEFINE sqlStatementName CHAR( m )
-- 將 SQL 語法放入變數內 --
LET sqlStatementName = "SQL Statement"
-- 宣告 Prepare 變數 --
PREPARE sqlPrepareName FROM sqlStatementName
-- 宣告游標 --
DECLARE cursorName SCROLL CURSOR [ WITH HOLD ] FOR sqlPrepareName
-- 開啟游標 --
OPEN cursorName [ USING variable1 [, variable2, ... ] ]
-- 透過控制游標，來顯示緩衝區的資料表資料 --
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
可能問題：

會造成暫存檔空間不足，且有資料不及時的問題發生。
{% endhint %}

{% hint style="info" %}
解決方式：

1. 同時使用 SCROLL CURSOR 敘述及 UPDATE CURSOR 敘述。
2. SCROLL CURSOR 敘述負責主鍵及提供游標移動。
3. UPDATE CURSOR 敘述依據 SCROLL CURSOR 敘述的主鍵，以取得完整資料。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
