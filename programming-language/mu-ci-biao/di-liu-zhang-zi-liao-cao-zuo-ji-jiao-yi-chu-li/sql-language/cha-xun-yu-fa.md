---
description: Informix-4GL 資料操作_SQL Language
---

# SELECT 語法

## 語法

```sql
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
               / columnName IN( Subquery )
               / EXISTS Subquery
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

1.  WHERE NOT clause：

    表示判斷結果依據為反向。
2.  columnName BETWEEN expr1 AND expr2：

    將有介於 expr1 到 expr2 範圍之間的資料表欄位資料 ( columnName ) ，篩選出來。
3.  columnName IN( value \[, ...])：

    將資料表欄位資料 ( columnName ) 有符合 IN 之中的 value 資料塞選出來。
4.  expr IS NULL：

    判斷查詢結果是否為空值。
5.  columnName LIKE "expr"：

    將有符合 LIKE 條件的資料表欄位資料 ( columnName ) 塞選出來。

    1. %：資料若符合沒有或更多字元，就塞選出來。
    2. \_：資料只要符合指定的一個字元，就塞選出來。
    3. \：資料內含有 % 或 \_ ，就塞選出來。
6.  columnName MATCHES "expr"：

    將有符合 MATCHES 條件的資料表欄位資料 ( columnName ) ，塞選出來。

    1. \*：資料若符合沒有或更多字元，就塞選出來。
    2. ?：資料只要符合任一字元，就塞選出來。
    3. \[...]：資料只要符合一串字串中的任一字元，就塞選出來。
    4. ^：需與 \[...] 搭配使用，資料只要沒有符合一串字串中的任一字元，就塞選出來。
    5. \：資料內含有 \* 或 ? ，就塞選出來。
7. columnName IN( Subquery )：
   * 建立新的查詢 ( Subquery )，得到 Subquery 所搜尋到的資料，並將有符合前述查詢結果的資料表欄位資料 ( columnName ) ，塞選出來。
   * Subquery 只能設定單一欄位作為查詢依據，但可得到多筆資料，以進行對資料表欄位資料 ( columnName ) 的比對
8. EXISTS Subquery：
   * 建立新的查詢 ( Subquery )，得到 Subquery 所搜尋到的資料，並將有符合條件的資料 ，塞選出來。
   * Subquery 可選取多個欄位作為查詢依據，並將主要 SELECT 敘述所選取的欄位帶入，作為查詢條件，且 Subquery 所使用的欄位均為主要 SELECT 敘述內的欄位。
9.  ALL Subquery：


10. ANY Subquery：
11. SOME Subquery：
12. AND clause：
13. OR clause：
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
