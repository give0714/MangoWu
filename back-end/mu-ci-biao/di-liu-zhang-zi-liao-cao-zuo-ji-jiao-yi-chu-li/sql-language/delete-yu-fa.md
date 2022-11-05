---
description: Informix-4GL 資料操作_SQL Language
---

# DELETE 語法

## 語法

```sql
DELETE FROM tableName
[WHERE [ NOT ] booleanExpr
               / columnName BETWEEN expr1 AND expr2
               / columnName IN( value [, ...])
               / expr IS NULL
               / columnName LIKE "expr"
               / columnName MATCHES "expr"
               / columnName IN Subquery
               / columnName EXISTS Subquery
               / { ALL Subquery / ANY Subquery / SOME Subquery } -- 三則一 --
 [ AND clause ]
  [ OR clause ]]
```

{% hint style="info" %}
功能：

刪除資料表內資料。
{% endhint %}

{% hint style="info" %}
說明：

無法刪除部分欄位資訊，須使用 UPDATE，將欲刪除之欄位設定為 NULL。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
