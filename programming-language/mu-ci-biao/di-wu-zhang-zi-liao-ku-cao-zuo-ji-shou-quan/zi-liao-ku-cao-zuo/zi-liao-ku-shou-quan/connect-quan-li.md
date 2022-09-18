---
description: Informix-4GL 資料庫授權
---

# CONNECT 權利

## 語法\_所有使用者

```sql
-- 授予 CONNECT 權利--
GRANT  CONNECT TO   PUBLIC
-- 取消 CONNECT 權利--
REVOKE CONNECT FROM PUBLIC
```

## 語法\_指定使用者

```sql
-- 授予 CONNECT 權利--
GRANT  CONNECT TO   userName
-- 取消 CONNECT 權利--
REVOKE CONNECT FROM userName
```

{% hint style="info" %}
說明：

* CONNECT 權利無法新增或刪除資料庫內的資料表和索引。
* 需於 DATABASE 敘述設定。
* 允許一個以上的使用者共用。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
