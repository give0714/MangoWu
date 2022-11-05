---
description: Informix-4GL 資料庫連結
---

# 資料庫連結

## 語法

```sql
CONNECT TO ( databaseName [ AS databaseVariableName ]
                          [ USER ( userId / userIdVariable ) USING variableVar ]
             / DEFAULT )
           [ WITH CONCURRENT TRANSACTION ]
```

{% hint style="info" %}
說明：

variableVar：驗證對應帳號的密碼。

WITH CONCURRENT TRANSACTION：於連接交易事務時，可同時切換不同交易事務使用。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
