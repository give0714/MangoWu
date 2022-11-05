---
description: Informix-4GL 資料操作
---

# CONSTRUCT

## 語法一

```
CONSTRUCT BY NAME variableName ON tableName.columnName1 [, tableName.columnName2, ... ]
          [ ATTRIBUTE 子句 ]
          [ HELP 輔助說明編號 ]
          [ BEFORE { ( FIELD screenFieldName1 [, screenFieldName2, ... ] ) / CONSTRUCT }
                   ( 4GLstatement
                     / sqlStatement
                     / NEXT FIELD ( screenFieldName / NEXT / PREVIOUS )
                     / ( EXIT / CONTINUE ) INPUT ) ]
          [ AFTER { ( FIELD screenFieldName1, [, screenFieldName2, ... ] ) / CONSTRUCT }
                   ( 4GLstatement
                     / sqlStatement
                     / NEXT FIELD ( screenFieldName / NEXT / PREVIOUS )
                     / ( EXIT / CONTINUE ) INPUT ) ]
          [ ON KEY( keybordName )
                   ( 4GLstatement
                     / sqlStatement
                     / NEXT FIELD ( screenFieldName / NEXT / PREVIOUS )
                     / ( EXIT / CONTINUE ) INPUT ) ]
[ END CONSTRUCT ]
```

## 語法二

```
CONSTRUCT BY NAME variableName ON tableName.columnName1 [, tableName.columnName2, ... ]
                               FROM screenFieldName1 [, screenFieldName2, ... ]
          [ ATTRIBUTE 子句 ]
          [ HELP 輔助說明編號 ]
          [ BEFORE { ( FIELD screenFieldName1 [, screenFieldName2, ... ] ) / CONSTRUCT }
                   ( 4GLstatement
                     / sqlStatement
                     / NEXT FIELD ( screenFieldName / NEXT / PREVIOUS )
                     / ( EXIT / CONTINUE ) INPUT ) ]
          [ AFTER { ( FIELD screenFieldName1, [, screenFieldName2, ... ] ) / CONSTRUCT }
                   ( 4GLstatement
                     / sqlStatement
                     / NEXT FIELD ( screenFieldName / NEXT / PREVIOUS )
                     / ( EXIT / CONTINUE ) INPUT ) ]
          [ ON KEY( keybordName )
                   ( 4GLstatement
                     / sqlStatement
                     / NEXT FIELD ( screenFieldName / NEXT / PREVIOUS )
                     / ( EXIT / CONTINUE ) INPUT ) ]
[ END CONSTRUCT ]
```

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
