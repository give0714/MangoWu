---
description: Informix-4GL INPUT 敘述說明
---

# INPUT

## 語法一

```
INPUT ( variableName1 [, variableName2, ... ] / starVariable THEN endVariable )
    [ WITHOUT DEFAULTS ]
      FROM screenFiledName / screenRecordName.*
    [ ATTRIBUTE ]
    [ HELP helpName ]
    [ BEFORE ( FIELD fieldName / INPUT )
             ( 4GL_Statement
               / sqlStatement
               / NEXT FIELD ( fieldName / NEXT / PREVIOUS )
               / ( EXIT / CONTINUE ) INPUT )                ]
    [ AFTER ( FIELD fieldName / INPUT )
            ( 4GL_Statement
              / sqlStatement
              / NEXT FIELD ( fieldName / NEXT / PREVIOUS )
              / ( EXIT / CONTINUE ) INPUT )                ]
    [ ONKEY ( keybordName )
            ( 4GL_Statement
              / sqlStatement
              / NEXT FIELD ( fieldName / NEXT / PREVIOUS )
              / ( EXIT / CONTINUE ) INPUT )                ]
END INPUT
```

## 語法二

```
INPUT BY NAME starVariable THEN endVariable
    [ WITHOUT DEFAULTS ]
      FROM screenFiledName / screenRecordName.*
    [ ATTRIBUTE ]
    [ HELP helpName ]
    [ BEFORE ( FIELD fieldName / INPUT )
             ( 4GL_Statement
               / sqlStatement
               / NEXT FIELD ( fieldName / NEXT / PREVIOUS )
               / ( EXIT / CONTINUE ) INPUT )                ]
    [ AFTER ( FIELD fieldName / INPUT )
            ( 4GL_Statement
              / sqlStatement
              / NEXT FIELD ( fieldName / NEXT / PREVIOUS )
              / ( EXIT / CONTINUE ) INPUT )                ]
    [ ONKEY ( keybordName )
            ( 4GL_Statement
              / sqlStatement
              / NEXT FIELD ( fieldName / NEXT / PREVIOUS )
              / ( EXIT / CONTINUE ) INPUT )                ]
END INPUT
```

{% hint style="info" %}
說明

* WITHOUT DEFAULTS：在輸入時，會保留顯示原有變數，常用於修改資料時使用。
* HELP helpName：顯示輔助訊息說明。
*   BEFORE FIELD fieldName：

    觸發時機：輸入點移動到該畫面輸入欄位時，但在使用者開始輸入資料前，而觸發事件。

    使用時機：顯示訊息或初始值設定及顯示。
*   ONKEY ( keybordName )：

    觸發時機：使用者按下指定 keybordName 時。

    使用時機：提供即時輔助及說明。
*   AFTER FIELD fieldName：

    觸發時機：輸入點離開該畫面輸入欄位時，因使用者按指定案件後，而觸發事件。

    使用時機：使用者輸入該螢幕欄位後，所需的必要性檢查。

    指定案件：ACCEPT KEY

    &#x20;                 INTERRUPT KEY

    &#x20;                 ENTER KEY / TAB KEY

    &#x20;                 HOME KEY / END KEY

    &#x20;                 UP KEY / DOWN KEY / LEFT KEY / RIGTH KEY
* NEXT FIELD fieldName：迫使輸入點移動到螢幕欄位的 fieldName 。
* NEXT FIELD NEXT：迫使輸入點從目前螢幕欄位移動到下一個螢幕欄位。
* NEXT FIELD PREVIOUS：迫使輸入點從目前螢幕欄位移動到上一個螢幕欄位。
* CONTINUE INPUT：重新執行 INPUT 敘述。
* EXIT INPUT：結束 INPUT 敘述，執行 END INPUT 敘述後面的程式
{% endhint %}

{% hint style="warning" %}
執行順序

1. BEFORE INPUT
2. BEFORE FIELD fieldName
3. ONKEY( keybordName )
4. AFTER FIELD fieldName
5. AFTER INPUT
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
