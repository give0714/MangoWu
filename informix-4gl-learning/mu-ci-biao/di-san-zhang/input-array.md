---
description: Informix-4GL INPUT ARRAY 敘述說明
---

# INPUT ARRAY

```
INPUT ARRAY programArrayName [ WITHOUT DEFAULTS ]
      FROM screenArrayName.*
    [ ATTRIBUTE ]
    [ HELP helpName ]
    [ BEFORE ( FIELD [ fieldName ] / INPUT / DELECT / INSERT / ROW )
             ( 4GL_Statement
               / NEXT FIELD ( fieldName / NEXT / PREVIOUS )
               / ( EXIT / CONTINUE ) INPUT )                         ]
    [ AFTER ( FIELD [ fieldName ] / INPUT / DELECT / INSERT / ROW )
            ( 4GL_Statement
              / NEXT FIELD ( fieldName / NEXT / PREVIOUS )
              / ( EXIT / CONTINUE ) INPUT )                         ]
    [ ONKEY ( keybordName )
            ( 4GL_Statement
              / NEXT FIELD ( fieldName / NEXT / PREVIOUS )
              / ( EXIT / CONTINUE ) INPUT )                ]
END INPUT
```

{% hint style="info" %}
說明

* WITHOUT DEFAULTS：在輸入時，會保留顯示原有變數，常用於修改資料時使用。
* HELP helpName：顯示輔助訊息說明。
*   BEFORE INPUT：

    觸發時機：顯示預設資料後，但在使用者輸入前。

    使用時機：告知使用者如何輸入或初始值設定及顯示。
*   BEFORE ROW：

    觸發時機：

    1. 游標移動到下一個新列時。
    2. 空間不夠，造成 INSERT 敘述指令失效時。
    3. 按下 INTERRUPT 或 QUIT 後，造成 INSERT 敘述指令中斷時。
    4. 按下 DELETE 時。
*   BEFORE DELETE：

    觸發時機：使用者按下 DELETE ，刪除 SCREEN FORM 上的陣列資料後，但尚未執行資料庫刪除紀錄。

    使用時機：使用者選取螢幕欄位資料要做刪除時，但資料庫規則並不允許此資料被刪除，可在此阻止這種不正常刪除行為發生。

    可配合使用 EXIT INPUT 敘述或 CANCEL DELETE 敘述，並提供訊息。
*   BEFORE INSERT：

    觸發時機：

    1. 使用者開始輸入一筆新資料進陣列時。
    2. 按下 INSERT ，做新增資料至 SCREEN FORM 上的陣列時。
    3. 使用者移動游標，至陣列最後面開始另一空白螢幕陣列時。

    使用時機：取得或設定欄位值，並將其顯示。

    可配合使用 CANCEL INSERT 敘述，取消使用者的新增工作。
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
*   AFTER INSERT：

    觸發時機：當使用者新增一筆新資料進陣列後，將游標移動到下一個新的螢幕陣列前。
*   AFTER DELETE：

    觸發時機：按下 DELETE ，刪除一筆螢幕陣列紀錄後。
*   AFTER ROW：

    觸發時機：

    1. 使用者按下任一按鍵，移動游標離開目前的螢幕紀錄時。
    2. 使用者按下 ENTER / TAB ，移動游標離開目前螢幕紀錄時。
    3. 使用者按下 ACCEPT ，移動游標離開目前螢幕紀錄時。
    4. 使用者按下 INTERRUP ，移動游標離開目前的螢幕紀錄時。
    5. 使用者按下 INSERT ，移動游標離開目前的螢幕紀錄時。
*   AFETR INPUT：

    觸發時機：

    1. 使用者按下 ACCEPT ，而結束 INPUT ARRAY 指令，但尚未結束。
    2. 使用者按下 INTERRUP ，而結束 INPUT ARRAY 指令，但尚未結束。
    3. 使用者按下 QUIT ，而結束 INPUT ARRAY 指令，但尚未結束。

    使用時機：搭配 GET\_FLDBUF( ) 或 FIELD\_TOUCHED( ) 去檢查、修改或儲存使用者輸入的值，會與 NEXT FIELD 敘述一起使用。
* NEXT FIELD fieldName：迫使輸入點移動到螢幕欄位的 fieldName 。
* NEXT FIELD NEXT：迫使輸入點從目前螢幕欄位移動到下一個螢幕欄位。
* NEXT FIELD PREVIOUS：迫使輸入點從目前螢幕欄位移動到上一個螢幕欄位。
* CONTINUE INPUT：重新執行 INPUT ARRAY 敘述。
* EXIT INPUT：結束 INPUT ARRAY 敘述，執行 END INPUT 敘述後面的程式
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】\
如有建議芒果改進的地方，請前往芒果留言區留言\
使芒果與你們一起成長進步
{% endhint %}
