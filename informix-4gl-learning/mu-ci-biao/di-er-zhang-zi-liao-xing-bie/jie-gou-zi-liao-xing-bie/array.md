---
description: Informix-4GL 資料型別說明_ARRAY 資料型態
---

# ARRAY

## 語法一

```objectivec
DEFINE arrayName ARRAY[ i(, j(, k ))] OF datatype
```

宣告一個自訂名稱及資料型別的多維陣列

## 語法二

```bash
DEFINE arrayName ARRAY[ n ] RECORD
       variableName1 datatype
    [, variableName2 datatype
     , ...                    ]
END RECORD
```

宣告一個含以上的變數，放入陣列中

{% hint style="warning" %}
####  用法

* 如在執行使用陣列時，需使用 ESC 鍵，方能離開此次陣列，執行後續程式
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

**待建置陣列專用之庫存函數的章節**

