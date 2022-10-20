---
description: Informix-4GL 資料表操作_資料表授權
---

# 資料表授權

## 語法\_所有使用者

```sql
-- 授予權利--
GRANT  tablePrivilege ON tableName TO   PUBLIC
-- 取消權利--
REVOKE tablePrivilege ON tableName FROM PUBLIC
```

## 語法\_指定使用者

```sql
-- 授予權利--
GRANT  tablePrivilege ON tableName TO   userName
-- 取消權利--
REVOKE tablePrivilege ON tableName FROM userName
```

{% hint style="info" %}
tablePrivilege  授權種類：

1. INSERT
2. SELECT
3. ALTER
4. UPDATE
5. DELETE
6. INDEX
7. ALL
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
