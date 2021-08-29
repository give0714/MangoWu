---
description: Informix-4GL 報表架構說明《一》
---

# START REPORT

```objectivec
START REPORT reportName
    [ TO ( SCREEN / PRINTER / [ FILE ] fileName ) ]
    / ( PIPE programName [ IN FORM / IN LINE ] [ MODE ] )
    / OUTPUT ( variableName 
               / "SCREEN" 
               / "PRINTER" )
               / ( ( variableName 
                     / "FILE" 
                     / "PIPE [ ( [ IN FORM / IN LINE ] ) MODE ]" )
                     / ( DESTINATION "programName" 
                         / "fileName" ) )        
      [ WITH
             PAGE   LENGTH  [ = ] num
             TOP    MARGIN  [ = ] num
             BOTTOM MARGIN  [ = ] num
             RIGTH  MARGIN  [ = ] num
             LEFT   MARGIN  [ = ] num
             TOP    OF PAGE [ = ] "str" ]
```

{% hint style="info" %}
目的

設定 reportName 頁面配置，指定報表輸出方式
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

