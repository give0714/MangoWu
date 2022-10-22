---
description: Informix-4GL 資料操作_QBE
---

# 變數與欄位名稱不相同

## 語法

```inform7
--  --
DEFINE sqlStatementName CHAR( m )
--  --
OPEN FORM formName FROM "formFileName"
--  --
DISPLAY FROM formName [ Attribute ]
--  --
CONSTRUCT BY NAME variableName ON tableName.columnName1 [, tableName.columnName2, ... ]
                               FROM screenFieldName1 [, screenFieldName2, ... ]
...
--  --
LET sqlStatementName = "SQL Statement",
                       "WHEWE ", variableName CLIPPED
--  --
PREPARE sqlPrepareName FROM sqlStatementName
--  --
DECLARE cursorName CURSOR FOR selPrepareName
--  --
OPEN cursorName [ USING variableName1 [, variableName2, ... ] ]
--  --
FETCH [ NEXT
        / ( PREVIOUS / PRIOR )
        / FIRST
        / LAST
        / CURRENT
        / RELATIVE m
        / ABSOLUTE n ] cursorName INTO selectTableName.*
--  --
CLOSE cursorName
--  --
FREE cursorName
--  --
CLOSE FORM formName
```

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
