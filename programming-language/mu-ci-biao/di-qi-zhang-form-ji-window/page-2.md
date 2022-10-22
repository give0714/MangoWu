---
description: Informix-4GL 畫面操作說明
---

# FORM SECTION

## DATABASE Section

```inform7
DATABASE databaseName
         / FORMONLY
```

{% hint style="info" %}
目的：

設定 SCREEN FORM 使用哪個資料庫。
{% endhint %}

{% hint style="info" %}
說明：

DATABASE FORMONLY：與任何資料庫沒有關聯，且 TABLE Section 可省略不寫。
{% endhint %}

## SCREEN Section

```inform7
SCREEN [ SIZE m [ BYTE n ] ]
{
  FORM Designer
}
END
```

{% hint style="info" %}
目的：

設定 SCREEN FORM 執行樣貌。
{% endhint %}

{% hint style="info" %}
說明：

SIZE m：設定螢幕顯示總列數量，m 為正整數值，預設 24 列。

BYTE n：設定螢幕顯示每列最大字元數量，n 為正整數值。
{% endhint %}

## TABLE Section

```inform7
TABLE [ alias = ] tableName [ END ]
```

{% hint style="info" %}
目的：

設定 SCREEN FORM 使用資料庫內哪些資料表。
{% endhint %}

## TABLE Section

### 語法一\_有參照資料庫資料表中欄位

```inform7
ATTRIBUTER
          fieldName = tableName.columnName [, Attribute, ... ]
          ...
END
```

### 語法二\_無參照資料庫資料表中欄位

```
ATTRIBUTER
          fieldName = FORMONLY.screenFormColumnName
                      ( [ type datatype [ NOT NULL ]
                                        / TYPE LIKE tableName.columnName ] )
                        [, Attribute, ... ]
          ...
END
```

{% hint style="info" %}
目的：

設定 SCREEN FORM 各螢幕欄位的特性。
{% endhint %}

## INSTRUCTIONS Section

```inform7
INSTRUCTIONS
            [ DELIMITERS "起始邊界符號"結束邊界符號" ]
            [ SCREEN RECORD recordName ( ( [ tableName ].*
                                           / 1stColumnName, 2stColumnName, ...
                                           / 1stColumnName ( THROUGH / TURN )
                                             [ tableName ].lastColumnName ) ) ]
            [ SCREEN RECORD arrayName[n] ( fieldList ) ]
[ END ]
```

{% hint style="info" %}
目的：

為選擇性設定，定義 SCREEN FORM、定義 SCREEN ARRAYS、改變 field tag 邊界符號。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
