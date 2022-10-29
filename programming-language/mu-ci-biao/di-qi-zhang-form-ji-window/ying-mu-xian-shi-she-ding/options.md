---
description: Informix-4GL 畫面操作說明
---

# OPTIONS

## 語法

```inform7
OPTIONS
        [ COMMENT LINE ( FIRST ( +  / - ) ( number ) 
                         / LAST ( +  / - ) ( number )
                         / number ) ]
        [ ERROR   LINE ( FIRST ( +  / - ) ( number ) 
                         / LAST ( +  / - ) ( number )
                         / number ) ]
        [ FORM    LINE ( FIRST ( +  / - ) ( number ) 
                         / LAST ( +  / - ) ( number )
                         / number ) ]
        [ MENU    LINE ( FIRST ( +  / - ) ( number ) 
                         / LAST ( +  / - ) ( number )
                         / number ) ]
        [ MESSAGE LINE ( FIRST ( +  / - ) ( number ) 
                         / LAST ( +  / - ) ( number )
                         / number ) ]
        [ PROMPT  LINE ( FIRST ( +  / - ) ( number ) 
                         / LAST ( +  / - ) ( number )
                         / number ) ]
        [ ACCEPT   KEY keybordName ]
        [ DELETE   KEY keybordName ]
        [ INSERT   KEY keybordName ]
        [ NEXT     KEY keybordName ]
        [ PREVIOUS KEY keybordName ]
        [ HELP     KEY keybordName ]
        [ HELP FILE "fileName" ]
        [ DISPLAY Attribute ]
        [ INPUT   Attribute ]
        [ INPUT [ NO ] WRAP ]
        [ FIELD ORDER ( UNCONSTRAINED / CONSTRAINED ) ]
        [ SQL INTERRUPT ( ON / OFF ) ]
        [ PIPE ( IN FORM MODE
                 / IN LINE MODE ) ]
        [ RUN  ( IN FORM MODE
                 / IN LINE MODE ) ]
```

{% hint style="info" %}
說明

* ACCEPT KEY \~ HELP KEY：\
  設定上述六種功能之自訂按鍵。\
  若無設定，系統會以預設值為主。
* COMMENT LINE \~ PROMPT LINE：\
  設定上述六種說明行的位置。\
  若無設定，系統會以預設值為主。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
