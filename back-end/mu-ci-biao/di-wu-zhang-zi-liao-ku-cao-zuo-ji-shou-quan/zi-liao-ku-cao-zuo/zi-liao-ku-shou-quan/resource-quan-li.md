---
description: Informix-4GL 資料庫授權
---

# RESOURCE 權利

## 語法\_所有使用者

```sql
-- 授予 RESOURCE 權利--
GRANT  RESOURCE TO   PUBLIC
-- 取消 RESOURCE 權利--
REVOKE RESOURCE FROM PUBLIC
```

## 語法\_指定使用者

```sql
-- 授予 RESOURCE 權利--
GRANT  RESOURCE TO   userName
-- 取消 RESOURCE 權利--
REVOKE RESOURCE FROM userName
```

{% hint style="info" %}
說明：

* RESOURCE 權利具有新增或刪除資料庫內的資料表和索引。
* 需於 DATABASE 敘述設定。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
