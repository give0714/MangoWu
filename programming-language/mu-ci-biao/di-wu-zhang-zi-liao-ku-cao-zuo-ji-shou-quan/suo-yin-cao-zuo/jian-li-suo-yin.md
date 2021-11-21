---
description: Informix-4GL 索引操作
---

# 建立索引

## 語法

```
CREATE [( UNIQUE / DISTINCT )[ CLUSTER ]] INDEX indextName ON tableName
        ( columnName1 datatype [ desc ],
          columnName2 datatype [ desc ], ...)
       [ FILLFACTOR n% ][ IN dbspace ]
       [( DIABLED / ENABLED / FILTERING )[( WITHOUT ERROR / WITH ERROR )]]
```

{% hint style="info" %}
說明：

UNIQUE / DISTINCT：可避免使用者輸入相關資訊。

欲使程式因錯誤而不被終止，需加入下述敘述

1. DEFER INTERRUPT。
2. INSERT INTO 前，加上 WITH ERROR CONTINUE。
3. INSERT INTO 後，加上 IF status = -239 THEN ... END IF
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
