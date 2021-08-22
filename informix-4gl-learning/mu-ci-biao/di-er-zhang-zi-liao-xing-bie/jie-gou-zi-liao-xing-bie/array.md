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

* 存取所有 RECORD variables recordName.\*
* 存取指定範圍 RECORD variable recordName.beginVariable THRU recordName.endVariable
* 存取單一 RECORD variable recordName.variableName
{% endhint %}

