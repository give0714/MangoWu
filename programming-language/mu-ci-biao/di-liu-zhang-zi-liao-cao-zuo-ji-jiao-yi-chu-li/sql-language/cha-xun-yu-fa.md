---
description: Informix-4GL 資料操作_SQL Language
---

# SELECT 語法

## 語法

```inform7
SELECT [ FIRST m ][ DISTINCT / UNIQUE ]
       *
       / columnName [ AS displayLabel ][, ...]
       / expr [ AS displayLabel1 ]
[ INTO recordName.* / variableName [, ...]
  FROM tableName [[ AS ] alias ][, ...]
[OUTER joinTableName1 [, OUTER joinTableName2 [, ...]]]
[WHERE [ NOT ] booleanExpr
               / columnName BETWEEN expr1 AND expr2
               / columnName IN( value [, ...])
               / expr IS NULL
               / columnName LIKE "expr"
               / columnName MATCHES "expr"
               / columnName IN Subquery
               / columnName EXISTS Subquery
               / { ALL Subquery / ANY Subquery / SOME Subquery } -- 三擇一 --
 [ AND clause ]
  [ OR clause ]]
[GROUP BY columnName [, ...]/ p [ HAVING booleanExpr ]]
[ORDER BY { columnName [, ...]/ n / column i, j } -- 三擇一 --
          [ ASC / DESC ]]
 [ FOR READ ONLY [ OF column [, ...]]
   / FOR UPDATE [ OF column [, ...]]]
[ INTO TEMP tableName [ WITH NO LOG]
       / SCRATCH tableName
       / EXTERNAL tableName USING Subquery ]
[UNION [ ALL ] Subquery ] 
```

{% hint style="info" %}
功能：

查詢資料表內資料。
{% endhint %}

{% hint style="info" %}
Subquery 用法說明：

1.  FIRST m：取得查詢結果的前 m 筆資料。

    m 為數值。
2. DISTINCT：如果查詢到重覆相同值的資料時，只會選取其中一筆資料顯示。
3. columnName AS displayLabel ：displayLabel 為 columnName 的欄位名稱敘述。
4.  FROM tableName AS aliasl：設定 tableName 為資料查詢來源。

    aliasl 為 tableName 的別名。
5. OUTER joinTableName：用於連結其他外部資料表，joinTableName 為外部資料表，無論是否有相對應的資料，都會將其顯示。
6. WHERE clause：請參考 clause 用法說明。
7.  GROUP BY columnName / p：依據 columnName 或 p 做分類群組。

    p 為數值或某個代表分類意義。
8. HAVING booleanExpr：須與 GROUP BY 同時搭配使用，表示查詢資料須符合 booleanExpr 的條件式判斷，才能被 GROUP BY 分類敘述。
9.  ORDER BY：查詢結果依據 columnName 或 n 或 column 的起始字元  i \~ 結束字元 j，來做升冪或降冪排序。

    n 為數值或某的具有代表意義。

    i、j 為數值。
10. ASC：升幕排序，系統預設。
11. DESC：降幕排序。
12. FOR READ ONLY：設定查詢結果只能讀取特性，不可修改，可設定一個以上的欄位具有此特性。
13. FOR UPDATE：設定查詢結果為可修改特性，可設定一個以上的欄位具有此特性。
14. INTO TEMP tableName \[ WITH NO LOG ]：將查詢結果存到一個暫存檔內。
15. INTO SCRATCH tableName：了解中。
16. INTO EXTERNAL tableName USING Subquery：了解中。
17. UNION Subquery：將查詢結果與 Subquery 的查詢結果做資料聯集，但搜尋的欄位數量及欄位資料型別兩邊都需一致，且不可以是 BYTE 或 TEXT 的資料型別。
18. UNION ALL Subquery：將查詢結果與 Subquery 的查詢結果做資料聯集，但搜尋的欄位數量及欄位資料型別兩邊都需一致。
{% endhint %}

{% hint style="info" %}
clause 用法說明：

1. WHERE NOT clause：表示判斷結果依據為反向。
2. columnName BETWEEN expr1 AND expr2：檢查 columnName 是否介於 expr1 到 expr2 範圍之間。
3.
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
