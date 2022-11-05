---
description: Informix-4GL 資料操作_QBE
---

# 變數與欄位名稱相同

## 語法

```
-- 宣告 SQL 語法變數 --
DEFINE sqlStatementName CHAR( m )
-- 開啟顯示窗 --
OPEN FORM formName FROM "formFileName"
-- 將變數顯示在對應的畫面上 --
DISPLAY FROM formName [ Attribute ]
-- 輸入變數資訊，並顯示在畫面上指定相同名稱的欄位 --
CONSTRUCT BY NAME variableName ON tableName.columnName1 [, tableName.columnName2, ... ]
...
-- 組合 SQL 語法 --
LET sqlStatementName = "SQL Statement",
                       "WHEWE ", variableName CLIPPED
-- 宣告 Prepare 變數 --
PREPARE sqlPrepareName FROM sqlStatementName
-- 宣告游標 --
DECLARE cursorName SCROLL CURSOR FOR selPrepareName
-- 開啟游標 --
OPEN cursorName [ USING variableName1 [, variableName2, ... ] ]
-- 取得游標所在位置的資料庫資料 --
FETCH [ NEXT
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
-- 關閉畫面 --
CLOSE FORM formName
```

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
