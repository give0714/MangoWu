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
END RECORD
```

宣告一個紀錄，內含一個含以上的變數

{% hint style="warning" %}
#### &#x20;用法

* 存取所有 RECORD variables\
  recordName.\*
* 存取指定範圍 RECORD variable\
  recordName.beginVariable THRU recordName.endVariable
* 存取單一 RECORD variable\
  recordName.variableName
{% endhint %}

{% hint style="danger" %}
【 [M@nGo 留言區](https://give0714.pixnet.net/blog/post/46468375-informix-4gl-%E7%B5%90%E6%A7%8B%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-record-data-%E3%80%8B) 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
