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
#### &#x20;用法

* 如在執行使用陣列時，需使用 ESC 鍵，方能離開此次陣列，執行後續程式
{% endhint %}

{% hint style="danger" %}
【 [M@nGo 留言區](https://give0714.pixnet.net/blog/post/46468651-informix-4gl-%E7%B5%90%E6%A7%8B%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-array-data-%E3%80%8B) 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
