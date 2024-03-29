---
description: Informix-4GL 畫面操作說明
---

# ATTRIBUTE 種類

<details>

<summary>AUTONEXT</summary>

若該欄資料輸入填滿，系統自動換下一欄位，無須按 ENTER

</details>

<details>

<summary>COLOR = Attribute [ WHERE clause ]</summary>

設定該欄位的顏色或文字粗細。

</details>

<details>

<summary>COMMENTS = "string"</summary>

顯示 string 於螢幕 SCREEN 第 23 行上，通常設定注意或提示訊息。

</details>

<details>

<summary>DEFAULT = systemVariable</summary>

systemVariable 為系統變數或常數。

</details>

<details>

<summary>DISPLAY LIKE tableName.columnName</summary>

設定該欄位資訊參照 tableName.columnName。

</details>

<details>

<summary>DOWNSHIFT</summary>

設定該欄位的所有英文字元轉換成小寫。

</details>

<details>

<summary>UPSHIFT</summary>

設定該欄位的所有英文字元轉換成大寫。

</details>

<details>

<summary>FORMAT = "formatString"</summary>

控制輸出時該欄位的顯示格式。

</details>

<details>

<summary>PICTURE = "formatString"</summary>

控制輸入時的該欄位的顯示格式。

</details>

<details>

<summary>INCLUDE = ( value [ TO value ] / NULL )</summary>

設定該欄位的值域，並將此值當該欄位的檢查依據。

</details>

<details>

<summary>INVISIBLE</summary>

設定在輸入資料時，不會顯示在螢幕上。

通常使用於密碼輸入。

</details>

<details>

<summary>NOENTRY</summary>

若該欄位設定為 NOENTRY 屬性，於輸入時，是無法輸入資料。

</details>

<details>

<summary>PROGRAM = "command"</summary>

設定該欄位去執行外部應用程式。

常發生於 TEXT 或 BYTE 的欄位時。

</details>

<details>

<summary>REQUIRED</summary>

強迫使用者輸入資料。

若有設定 DEFAULT 時，此時 REQUIRED 為無效。

</details>

<details>

<summary>REVERSE</summary>

設定該欄位反白。

</details>

<details>

<summary>VALIDATE LIKE [ tableName. ] colunmName</summary>

於輸入資料後，檢查的依據此屬性之設定。

</details>

<details>

<summary>VERIFY</summary>

強迫使用者輸入兩次，並比較兩次輸入是否一致。

</details>

<details>

<summary>WORDWRAP [ COMPRESS / NONCOMPRESS ]</summary>

於 CHAR 的欄位資料，且長度超過 58 byte 時，設定有無需要切割顯示。

</details>

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
