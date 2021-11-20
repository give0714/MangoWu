---
description: Informix-4GL 庫存函數_錯誤型使用說明
---

# STARTLOG( )

## 語法

```
STARTLOG( fileName )
```

{% hint style="info" %}
目的：

開啟錯誤日誌檔案。
{% endhint %}

{% hint style="info" %}
說明：

fileName ： 字串或 CHAR 資料型態的變數，為錯誤日誌檔名。

檔案若不存在，系統會建立檔案及依 fileName 來命名檔案。

建議設定錯誤日誌檔案的完整路徑。

若使用此函數後，後續均會記錄發生之錯誤訊息，並將資訊寫入檔案內。

檔案內含錯誤日期、時間、原始程式碼、程式行數、錯誤編號、錯誤訊息等資訊。

可利用 ERRORLOG( ) 寫入自定義之錯誤訊息。
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】\
如有建議芒果改進的地方，請前往芒果留言區留言\
使芒果與你們一起成長進步
{% endhint %}
