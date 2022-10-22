---
description: Informix-4GL 資料操作_QBE 說明
---

# QBE 說明

## 簡稱

Query By Example < QBE >

## 目的

透過 SCREEN FORM 的欄位，可讓使用者輸入欲查詢的資料，並透過組合方式，\
將資料轉換成 SELECT 敘述的 SQL 語法。

## 使用前提

1. 必須有 FORM 被 OPEN 或 DISPLAY，且有連結資料庫。
2. 宣告一個長度很長的 CHAR 資料型別變數，以備承接輸入的查詢條件。
3. 如有多個 FORM 被開啟，需選擇正確 SCREEN FORM，\
   通常用 CURRENT WINDOW 來指定特定 FORM。

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
