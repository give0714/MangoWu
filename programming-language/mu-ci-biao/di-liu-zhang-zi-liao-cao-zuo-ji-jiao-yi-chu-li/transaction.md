---
description: Informix-4GL 資料操作
---

# Transaction

## 語法

```sql
CREATE DATABASE databaseName WITH LOG IN "pathName"
...
START DATABASE
...
BEGIN WORK
...
COMMIT WORK
...
ROLLBACK WORK
```

{% hint style="info" %}
說明：

WITH LOG IN 敘述：\
建立可使用交易的資料庫。

BEGIN WORK 敘述：\
置於群組第一敘述之前。\
如敘述執行失敗，系統會自行回復執行前的狀態。\
如無使用此敘述，系統會將每一敘述視為單一交易。

COMMIT WORK 敘述：\
置於群組最後敘述之後。\
如執行敘述成功，則會停止交易。

ROLLBACK WORK 敘述：\
置於群組最後敘述之後。\
如執行敘述失敗，則會回復成 BEGIN WORK 敘述之前的資料庫狀態。
{% endhint %}

## 復原損毀的資料庫

```sql
ROLLFORWARD DATABASE databaseName
```



{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
