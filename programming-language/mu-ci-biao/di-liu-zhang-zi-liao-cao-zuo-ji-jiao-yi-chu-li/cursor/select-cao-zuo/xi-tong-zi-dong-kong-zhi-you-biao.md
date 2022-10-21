---
description: Informix-4GL 資料操作_游標
---

# 系統自動控制游標

## 語法

```sql
-- 宣告變數 --
DEFINE recordTableName RECORD LIKE tableName.*
-- 宣告游標 --
DECLARE cursorName CURSOR FOR
        SELECT * FROM tableName
-- 開啟游標 --
FOREACH cursorName INTO selectTableName.*
        ...
        CONTINUE FOREACH
        ...
        EXIT FOREACH
        ...
END FOREACH
-- 釋放游標 --
FREE cursorName
```

{% hint style="info" %}
流程說明：

1.  DECLARE 游標

    取得記憶體空間，以放置 CURSOR 游標，並將其指向 NULL〈指標 Point〉。
2.  FOREACH 游標

    系統會自己控制開啟游標及關閉游標的時機，且執行過程為依查詢結果，依序將結果寫入\
    資料緩衝區的記憶體空間。\
    CONTINUE FOREACH 為中斷此次結果，跳到下一次 FOREACH 敘述程式的查詢結果。\
    EXIT FOREACH 為結束 FOREACH 敘述程式執行。
3.  FREE 游標

    釋放資料緩衝區的記憶體空間。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
