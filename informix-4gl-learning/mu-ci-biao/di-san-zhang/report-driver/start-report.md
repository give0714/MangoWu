---
description: Informix-4GL 報表架構說明《一》
---

# START REPORT

```objectivec
START REPORT reportName
    [ TO ( SCREEN 
           / PRINTER 
           / [ FILE ] fileName )]
    /( PIPE programName [ IN FORM / IN LINE ] [ MODE ] )
    / OUTPUT ( variableName 
               / "SCREEN" 
               / "PRINTER" )
               /(( variableName 
                   / "FILE" 
                   / "PIPE [ ( [ IN FORM / IN LINE ] ) MODE ]" )
                   /( DESTINATION "programName" 
                      / "fileName" ) )        
      [ WITH
             PAGE   LENGTH  [=] num
             TOP    MARGIN  [=] num
             BOTTOM MARGIN  [=] num
             RIGTH  MARGIN  [=] num
             LEFT   MARGIN  [=] num
             TOP    OF PAGE [=] "str" ]
```

{% hint style="danger" %}
建置中
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

