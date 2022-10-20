---
description: 宣告 Informix-4GL 變數的多種語法
---

# 宣告變數

## 語法一

```objectivec
DEFINE variableName1 datatype
    (, variableName2 datatype
     , ...                    )
```

宣告一個（含以上）自訂名稱及資料型別的變數

## 語法二

```bash
DEFINE variableName LIKE tableName.columnName
```

宣告繼承某資料表之特定欄位屬性的變數

## 語法三

```bash
DEFINE recordName RECORD LIKE tableName.*
```

宣告一個紀錄，內含繼承某資料表所有欄位

## 語法四

```bash
DEFINE recordName RECORD
       variableName1 datatype
    (, variableName2 datatype
     , ...                    )
END RECORD
```

宣告一個紀錄，內含一個（含以上）自訂名稱及資料型別之變數

## 語法五

```bash
DEFINE arrayName ARRAY[ m(, n) ] OF RECORD
       variableName1 datatype
    [, variableName2 datatype
    [, ...                    ]
END RECORD
```

宣告一個陣列，內含一個（含以上）自訂名稱及資料型別之變數\
可透過 m 或 n 的使用，來控制陣列的維度

{% hint style="info" %}
#### 說明

* variableName：自定義之變數名稱
* tableName：資料表名稱
* columnName：欄位名稱
* recordName：自定義之紀錄名稱
* arrayName：自定義之陣列名稱
* m：為整數值
* n ：為整數值
{% endhint %}

{% hint style="warning" %}
#### &#x20;注意事項

* 上述五種語法，必須放置於在 GLOBALS 敘述、 MAIN 敘述、 FUNCTION 敘述、 REPORT 敘述之中，或是介於DATABASE 敘述及 MAIN 敘述之間，且必須於所有程式語法起始前做宣告動作
* 使用語法二，若所繼承之 TABLE 內含有 SERIAL的資料型別的欄位時，系統會自動轉換成 INTEGER 的資料型別
{% endhint %}

{% hint style="danger" %}
【 [M@nGo 留言區](https://give0714.pixnet.net/blog/post/45993157-informix-4gl-%E8%AE%8A%E6%95%B8%E5%AE%A3%E5%91%8A) 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
