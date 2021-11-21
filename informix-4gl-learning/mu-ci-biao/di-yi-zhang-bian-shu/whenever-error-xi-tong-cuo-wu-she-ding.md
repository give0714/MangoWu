---
description: Informix-4GL 系統錯誤設定使用說明
---

# WHENEVER ERROR 系統錯誤設定

## 語法一

```objectivec
WHENEVER [ ANY ] ERROR STOP
```

{% hint style="info" %}
#### 說明

* 系統預設處理方式
* 當錯誤發生時，系統會將錯誤訊息顯示於螢幕的 ERROR 行上，並停止程式執行
{% endhint %}

## 語法二

```objectivec
WHENEVER [ ANY ] ERROR CONTINUE
```

{% hint style="info" %}
#### 說明

* 當錯誤發生時，系統將會避開此錯誤，執行後續程式，不會中斷程式執行
* 若無額外的輔助錯誤處理，可能會造成無法彌補的錯誤發生
* 通常於 SQL 指令後，加上 SQLCA.SQLCODE 的檢查判斷
{% endhint %}

## 語法三

```objectivec
WHENEVER [ ANY ] ERROR CALL functionName( )
```

{% hint style="info" %}
#### 說明

* 當錯誤發生時，系統會執行系統內建或自定義的函數
{% endhint %}

{% hint style="danger" %}
【 [M@nGo 留言區](https://give0714.pixnet.net/blog/post/46000348-informix-4gl-%E7%B3%BB%E7%B5%B1%E9%8C%AF%E8%AA%A4%E8%A8%AD%E5%AE%9A) 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
