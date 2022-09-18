---
description: Informix-4GL 資料表操作
---

# 建立資料表

## 語法

```sql
CREATE [ TEMP ] TABLE tableName
       ( columnName1 datatype [ columnLevelConstraint ],
         columnName2 datatype [ columnLevelConstraint ], ...
         [ tableLevelConstraint1 [, tableLevelConstraint2, ...]])
       [ IN dbspace ]
       [ LOCK MODE ( PAGE / ROW / TABLE )]
       [ EXTENT SIZE firstKbytes ]
       [ NEXT SIZE nextKbytes ]
```

{% hint style="info" %}
說明：

TEMP：建立暫存檔。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
