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
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/46000348-informix-4gl-%e7%b3%bb%e7%b5%b1%e9%8c%af%e8%aa%a4%e8%a8%ad%e5%ae%9a) 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

