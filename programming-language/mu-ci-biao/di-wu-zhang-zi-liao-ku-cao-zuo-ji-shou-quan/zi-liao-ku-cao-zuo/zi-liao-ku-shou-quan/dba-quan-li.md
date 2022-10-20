---
description: Informix-4GL 資料庫授權
---

# DBA 權利

## 語法\_指定使用者

```sql
-- 授予 DBA 權利--
GRANT  DBA TO   userName
-- 取消 DBA 權利--
REVOKE DBA FROM userName
```

{% hint style="info" %}
說明：

* Informix-4GL 系統於使用者建立資料庫的同時，自動設定 DBA 權利給該使用者。
* 具有新增、修改或刪除資料庫內的資料表和索引。
* 具有啟用和刪除資料庫的權利。
* 具有授權和取消 CONNECT權利、RESOURCE 權利及 DBA 權利。
* 僅有一個使用者擁有 DBA 權利，且該使用者無法自己取消 DBA 權利，須由其他 DBA 權利的使用者做權利刪除。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
