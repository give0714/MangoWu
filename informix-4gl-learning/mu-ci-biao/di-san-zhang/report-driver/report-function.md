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

* DEFINE Section：定義 reportName 所使用到的報表變數 使用時機 1. ON EVERY ROW 所產生的報表，每筆的紀錄值均需傳遞至此時 2. ORDER BY 的變數值時 3. AFTER GROUP OF 的變數值時
* OUTPUT Section：用法如同 START REPORT 敘述的設定相關頁面格式及輸出檔案方式等資訊，系統會以 START REPORT 敘述設定為主
* ORDER BY：
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

