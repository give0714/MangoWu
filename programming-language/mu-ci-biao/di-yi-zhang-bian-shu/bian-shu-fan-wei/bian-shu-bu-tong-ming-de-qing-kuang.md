---
description: Informix-4GL 變數均不同名稱的作用範圍
---

# 變數不同名的情況

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
        DEFINE variable_C datatype
END FUNCTION
```

變數影響範圍說明

| 敘述       | 變數          | 型態   | 影響範圍          |
| -------- | ----------- | ---- | ------------- |
| GLOBALS  | variable\_A | 全域變數 | MAIN、FUNCTION |
| MAIN     | variable\_B | 區域變數 | MAIN          |
| FUNCTION | variable\_C | 區域變數 | FUNCTION      |

{% hint style="danger" %}
【 [M@nGo 留言區](https://give0714.pixnet.net/blog/post/45997210-informix-4gl-%E8%AE%8A%E6%95%B8%E7%AF%84%E5%9C%8D) 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
