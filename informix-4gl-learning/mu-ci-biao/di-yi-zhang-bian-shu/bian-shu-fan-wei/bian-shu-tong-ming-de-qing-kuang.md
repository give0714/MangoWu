---
description: Informix-4GL 變數部分同名稱的作用範圍
---

# 變數同名的情況

## 語法

```objectivec
DATABASE
GLOBALS
       DEFINE variable_A datatype
END GLOBALS

MAIN
    DEFINE variable_B datatype
END MAIN

FUNCTION functionName( )
        DEFINE variable_A datatype
END FUNCTION
```

變數影響範圍說明

| 敘述 | 變數 | 型態 | 影響範圍 |
| :--- | :--- | :--- | :--- |
| GLOBALS | variable\_A | 全域變數 | MAIN |
| MAIN | variable\_B | 區域變數 | MAIN |
| FUNCTION | variable\_A | 區域變數 | FUNCTION |

{% hint style="danger" %}
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/45997294-informix-4gl-%e8%ae%8a%e6%95%b8%e7%af%84%e5%9c%8d-%28-%e4%ba%8c-%29) 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

