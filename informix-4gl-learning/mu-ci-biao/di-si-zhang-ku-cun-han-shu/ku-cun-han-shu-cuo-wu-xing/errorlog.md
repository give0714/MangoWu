---
description: Informix-4GL 庫存函數_錯誤型使用說明
---

# ERRORLOG( )

## 語法

```
CALL STARTLOG("fileName")
LET strExpr = ERR_GET( intExpr )
CALL ERRORLOG( strExpr )
```

{% hint style="info" %}
目的：

將錯誤訊息存入 LOG 錯誤日誌內

strExpr：為字串常數或 CHAR 資料型態變數，若不是上述資料型態，系統會自動轉換。
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】\
如有建議芒果改進的地方，請前往芒果留言區留言\
使芒果與你們一起成長進步
{% endhint %}
