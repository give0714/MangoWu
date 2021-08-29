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

* PAGE LENGTH：設定每頁輸出總列數，預設為 66 列
* TOP MARGIN：設定每頁上邊界，預設為 3 列
* BOTTOM MARGIN：設定每頁下邊界，預設為 3 列
* RIGTH MARGIN：設定每頁右邊界，預設為 132 字元
* LEFT MARGIN：設定每頁左邊界，預設為 3 字元
* TOP OF PAGE：設定每頁跳頁判別字元，以印表機預設為主
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

