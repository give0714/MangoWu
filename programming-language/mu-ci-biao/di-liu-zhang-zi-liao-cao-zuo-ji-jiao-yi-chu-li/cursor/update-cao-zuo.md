---
description: Informix-4GL 資料操作_游標
---

# UPDATE 操作

## 語法

```sql
-- 宣告游標 --
DECLARE cursorName CURSOR FOR
        SELECT *
          FROM tableName
           FOR UPDATE
UPDATE tableName SET columnName = expr [, ... ]
[ WHERE [ NOT ] booleanExpr
                / BETWEEN expr1 AND expr2
                / IN( value [, ... ] )
                / expr IS NULL
                / LIKE "expr"
                /MATCHES "expr"
                / IN Subquery
                / EXISTS Subquery
                / { ALL Subquery / ANY Subquery / SOME Subquery } -- 三則一 --
  [ AND clause ]
  [ OR clause ] ]
-- 關閉游標，並將與此游標相關的變數資料新增至資料庫內 --
CLOSE cursorName
-- 釋放游標 --
FREE cursorName
```

{% hint style="info" %}
無法更新之狀況：

1. 使用 SCROLL CURSOR。
2. 查詢 2 個以上的資料表〈JOIN table〉。
3. 查詢含有 Aggregate Function〈如 SUM..〉、GROUD BY、ORDER BY 時。
{% endhint %}

{% hint style="info" %}
鎖定欄位：

```
UPDATE tableName SET columnName = expr [, ...]
     [ WHERE CURRENT OF columnName ]
     [ WHERE clause ]
```
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
