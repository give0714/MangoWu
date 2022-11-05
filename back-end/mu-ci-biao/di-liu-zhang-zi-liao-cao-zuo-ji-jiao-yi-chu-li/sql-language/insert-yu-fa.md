---
description: Informix-4GL 資料操作_SQL Language
---

# INSERT 語法

## 語法

```sql
INSERT INTO tableName [ columnName1 [, columnName2, ...]]
            VALUES( valueName1, [ valueName2, ...])
```

{% hint style="info" %}
功能：

新增資料至資料表內。
{% endhint %}

{% hint style="info" %}
說明：

CHAR 或 DATE 資料型別的常數，需使用雙引號括住。

新增含 SERIAL 的行時，可設定非 NULL，但不可與表中所有列有相同行值，若設定為 0，系統會自動新增，若新增列中所有資料時，可省略或列出行名。

可使用 WHERE ERROR CONTINUE 及 status，藉此判斷是否有重覆新增。

可使用 IF，藉此判斷資料是否為 NULL。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
