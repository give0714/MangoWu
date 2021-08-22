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

