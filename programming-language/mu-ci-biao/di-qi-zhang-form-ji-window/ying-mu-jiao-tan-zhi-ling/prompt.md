---
description: Informix-4GL 畫面操作說明
---

# PROMPT

## 語法

```inform7
PROMPT ( "str" / variable ) [ Attribute ]
       FOR [ CHAR ] variable
       [ HELP helpNumber ]
       [ ON KEY ( keybordName ) 
                ( 4GLstatement / sqlStatement )
         END PROMPT ]
```

{% hint style="info" %}
目的：

顯示訊息於 PROMPT 行，可提供使用者輸入，並可在結構內撰寫程式。\
預設位置在 CURRENT WINDOW 第一行。\
FOR CHAR variable 只接受輸入一個字元，並放入指定變數。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
