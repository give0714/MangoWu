---
description: Informix-4GL 報表架構說明《五》
---

# REPORT FORMAT Setion

```objectivec
EXIT REPORT
```

{% hint style="info" %}
目的

中斷 reportName 作業流程
{% endhint %}

## 

```objectivec
NEED num LINES
```

{% hint style="info" %}
目的

偵測本頁剩餘列印數是否足夠接下來欲列印區段的總列數，如果不足，系統自行執行換頁
{% endhint %}

## 

```objectivec
PAUSE "String"
```

{% hint style="info" %}
目的

暫停輸出 REPORT 程式執行，並顯示提示訊息給使用者
{% endhint %}

## 

```objectivec
SKIP ( TO TOP OF PAGE / num ( LINE / LINES ))
```

{% hint style="info" %}
目的

插入空白列或換行
{% endhint %}

## 

```objectivec
PRINT
      [ 4GL_Statement ]
      [ COLUMN num ]
      [ PAGENO ]
      [ LINENO ]
      [ BYTE variable ]
      [ mathStatement ( SPACE / SPACES ) ]
      [[ GROUP ] ( PERCENT(*)
                   / COUNT(*)
                   / AVG( integerStatement / 區間)Statement
```

{% hint style="info" %}
目的

插入空白列或換行
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

