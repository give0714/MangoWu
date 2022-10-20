---
description: Informix-4GL 欄位操作
---

# 新增欄位

## 語法一\_欄位新增於最後

```sql
ALTER TABLE tableName ADD ( newColumnName1 datatype
                            [, newColumnName2 datatype, ...])
```

## 語法二\_欄位新增於指令欄位前

```
ALTER TABLE tableName ADD ( newColumnName1 datatype BEFORE oldColumnName [, ...])
```

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
