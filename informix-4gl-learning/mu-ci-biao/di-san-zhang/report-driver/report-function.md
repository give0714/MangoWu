---
description: Informix-4GL 報表架構說明《四》
---

# REPORT FUNCTION

## 語法

```objectivec
REPORT reportName ( [ variableName1 [, variable2, ... ] ] )
     [ DEFINE Section ]
     OUTPUT
          [ REPORT TO ( SCREEN / PRINTER / [ FILE ] fileName )
                        / PIPE [ IN FORM MODE / IN LINE MODE ] programName ]
          [ PAGE   LENGTH  [ = ] num ]
          [ TOP    MARGIN  [ = ] num ]
          [ BOTTOM MARGIN  [ = ] num ]
          [ RIGTH  MARGIN  [ = ] num ]
          [ LEFT   MARGIN  [ = ] num ]
          [ TOP    OF PAGE [ = ] "str" ]
   [ ORDER [ EXTERNAL ] BY variableName1 [ ASC / DESC ]
                        [, variableName2 [ ASC / DESC ], ... ] ]
     FORMAT
          [ FIRST PAGE HEADER
            ...                          ]
          [ PAGE HEADER
            ...                          ]
          [ BEFORE GROUP OF variableName
            ...                          ]
          [ AFTER GROUP OF variableName
            ...                          ]
          [ PAGE TRAILER
            ...                          ]
          [ ON LAST ROW
            ...                          ]
END REPORT
```

{% hint style="info" %}
目的

設定 reportName 輸出格式及提供資料的輸出
{% endhint %}

{% hint style="info" %}
說明

* DEFINE Section：定義 reportName 所使用到的報表變數 使用時機： 1. ON EVERY ROW 所產生的報表，每筆的紀錄值均需傳遞至此時 2. ORDER BY 的變數值時 3. AFTER GROUP OF 的變數值時
* OUTPUT Section：用法如同 START REPORT 敘述的設定相關頁面格式及輸出檔案方式等資訊，系統會以 START REPORT 敘述設定為主
* ORDER BY：設定 reportName 排序方式
* FIRST PAGE HEADER：設定報表第一頁表頭格式
* PAGE HEADER：設定報表每一頁表頭格式
* BEFORE GROUP OF variableName：設定在開始 variableName 的 GROUP 前，所要完成的動作，需先將 variableName 排序過 使用限制： 1. 不能使用 SKIP num LINES 於迴圈內 2. 不能使用 NEED 3. 使用 IF 敘述時，THEN 的列數需與 ELSE 的列數一致 4. 在 CASE 敘述、 FOR 敘述、 WHILE 敘述使用 PRINT 時，每一 PRINT 的結束皆使用 5. 不能使用 PRINT FILE
* ON EVERY ROW：設定每一筆 INPUT RECORD 的動作及報表顯示方式
* AFTER GROUP OF variableName：設定在結束 variableName 的 GROUP 後，所要完成的動作，需先將 variableName 排序過 執行時機： 1. variableName 值改變時 2. 更高階的 GROUP 的值改變時 3. 最後一筆被輸出，但在執行 PAGE TRAILER 及 ON LAST ROW 時
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

