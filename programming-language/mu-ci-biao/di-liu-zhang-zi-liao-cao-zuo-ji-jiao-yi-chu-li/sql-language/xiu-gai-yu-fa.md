---
description: Informix-4GL 資料操作_SQL Language
---

# 修改語法

## 語法一

```inform7
UPDATE tableName SET columnName = expr [, ...]
     [ WHERE CURRENT OF cursorName ]
     [ WHERE clause ]
```

## 語法二

```inform7
UPDATE tableName SET ( columnName ) = ( expr [, ...])
     [ WHERE CURRENT OF cursorName ]
     [ WHERE clause ]
```

## 語法三

```inform7
UPDATE tableName SET tableName.* = recordTableName.*
     [ WHERE CURRENT OF cursorName ]
     [ WHERE clause ]
```

{% hint style="info" %}
功能：

將資料更新至資料表內。
{% endhint %}

{% hint style="info" %}
說明：

expr：為常數、變數、行名，或以上三者之組合。

cause：為新增欄位的條件。

columnName 和 expr 的資料型別可以不用相同。

CHAR 或 DATE 資料型別的資料，須用雙引號括住。

若省略 WHERE 子句，系統會自動更新表中所有資料。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
