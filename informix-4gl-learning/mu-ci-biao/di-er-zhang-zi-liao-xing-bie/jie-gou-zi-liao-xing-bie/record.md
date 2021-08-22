---
description: Informix-4GL 資料型別說明_RECORD 資料型態
---

# RECORD

## 語法一

```objectivec
DEFINE recordName RECORD LIKE tableName.*
```

宣告一個紀錄，內含繼承某資料表所有欄位

## 語法二

```bash
DEFINE recordName RECORD
       variableName1 datatype
    [, variableName2 datatype
     , ...                    ]
```

宣告一個紀錄，內含一個含以上的變數

{% hint style="warning" %}
####  用法

* 存取所有 RECORD variables recordName.\*
* 存取指定範圍 RECORD variable recordName.beginVariable THRU recordName.endVariable
* 存取單一 RECORD variable recordName.variableName
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

