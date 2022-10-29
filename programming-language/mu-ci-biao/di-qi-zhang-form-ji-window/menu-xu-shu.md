---
description: Informix-4GL 畫面操作說明
---

# MENU 敘述

## 語法

```inform7
MENU "menuName"
     [ BEFORE MENU
              [ 4GL statement ]
              [ NEXT OPTION "optionName" ]
              [ ( HIDE / SHOW ) OPTION ( "optionName1" [, "optionName2", ... ] / ALL ) ]
              [ CONTINUE MENU ]
              [ EXIT MENU ] ]

     [ COMMAND "optionName" "instruction"
       / COMMAND KEY ( keybordName )
       / COMMAND KEY ( keybordName ) "optionName" "instruction"
              [ HELP helpNumber ]
              [ 4GL statement ]
              [ NEXT OPTION "optionName" ]
              [ ( HIDE / SHOW ) OPTION ( "optionName1" [, "optionName2", ... ] / ALL ) ]
              [ CONTINUE MENU ]
              [ EXIT MENU ] ]
END MENU
```

{% hint style="info" %}
說明

* MENU "menuName"：\
  一般用於顯示系統名稱。
* BEFORE MENU：\
  在顯示菜單前，先執行的程式指令。
* NEXT OPTION "optionName"：\
  指定游標前往 optionName 選項位置。\
  optionName 選項需在 COMMAND 敘述內，有被註明使用的選項。
* HIDE OPTION "optionName"：\
  隱藏 optionName 選項。
* HIDE OPTION ALL：\
  隱藏所有菜單選項。
* SHOW OPTION "optionName"：\
  顯示 optionName 選項。
* SHOW OPTION ALL：\
  顯示所有菜單選項。
* CONTINUE MENU：\
  重新執行 MENU 敘述。
* EXIT MENU：\
  結束 MENU 敘述，執行 END MENU 敘述後的程式。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
