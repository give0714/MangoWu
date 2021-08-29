---
description: Informix-4GL 程式架構說明
---

# 程式架構

```objectivec
DATABASE databaseName

GLOBALS
       DEFINE globalVariableName datatype
       ...
END GLOBALS

DEFINE programVariableName datatype
...

MAIN
    DEFINE mainVariableName datatype
    ...
    CALL functionName( mainVariableName )
    RETURNING programVariableName
    ...    
END MAIN

FUNCTION functionName( functionVariableName )
         DEFINE functionVariableName datatype
         ...
         RETURN functionVariableName
END FUNCTION

REPORT reportName( )
       DEFINE reportVariablieName datatype
       書寫方式請詳本章節..
END REPORT
```

{% hint style="warning" %}
說明

* DATABASE：定義程式資料，欲參考的資料庫名稱
* GLOBALS：宣告程式內主程式、函數、報表皆可使用之全域變數
* DATABASE 與 MAIN 兩者之間：宣告程式內主程式、函數、報表皆可使用之區域變數
* MAIN：主程式，所有程式執行的起點及終點，可宣告主程式內可使用的區域變數、執行函數、執行 SQL 語法、執行報表輸出
* FUNCTION：函數，可宣告函數內可使用的區域變數、執行函數、執行 SQL 語法、執行報表輸出
* REPORT：定義程式資料輸出之報表格式，可宣告報表內可使用的區域變數、執行函數、執行 SQL 語法
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

