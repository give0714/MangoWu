---
description: Informix-4GL 資料型別說明_Number 資料型態
---

# DECIMAL

#### 說明

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">&#x8A9E;&#x6CD5;</td>
      <td style="text-align:left">DECIMAL ( precision [, scale ] )</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">precision : &#x6240;&#x6709;&#x6578;&#x5B57;&#x500B;&#x6578;&#xFF0C;&#x4E0D;&#x542B;&#x5C0F;&#x6578;&#x9EDE;&#xFF0C;&#x9810;&#x8A2D;&#x70BA;
        16</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">
        <p>scale : &#x6240;&#x6709;&#x5C0F;&#x6578;&#x9EDE;&#x53F3;&#x908A;&#x7684;&#x6578;&#x5B57;&#x500B;&#x6578;</p>
        <p>&#x9810;&#x8A2D;&#x7BC4;&#x570D; 10(-128) ~ 10(126)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8CC7;&#x6599;&#x9577;&#x5EA6;</td>
      <td style="text-align:left">
        <p>byte = ROUND ( precision / 2 + 1 )</p>
        <p>1.DECIMAL ( precision )</p>
        <p>1+ precision / 2 byte</p>
        <p>2.DECIMAL ( precision [, scale ] )</p>
        <p>scale &#x70BA;&#x5947;&#x6578; ( precision + 3 ) / 2 byte</p>
        <p>scale &#x70BA;&#x5076;&#x6578; ( precision + 4 ) / 2 byte</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8CC7;&#x6599;&#x7BC4;&#x570D;</td>
      <td style="text-align:left">32&#x500B;&#x6578;&#x5B57;&#x500B;&#x6578;</td>
    </tr>
  </tbody>
</table>

#### 範例一

```objectivec
DEFINE unitPrice DECIMAL
...
LET unitPrice = 1048.14
```

說明 : unitPrice 為預設 16 個數字個數的浮點數，內含 2 個小數點數值的浮點數

#### 範例二

```objectivec
DEFINE unitPrice DECIMAL( 9 )
...
LET unitPrice = 8791211.14
```

說明 : unitPrice 為有 9 個數字個數的浮點數

#### 範例三

```objectivec
DEFINE unitPrice DECIMAL( 7, 3 )
...
LET unitPrice = 4211.012
```

說明 : unitPrice 為有 7 個數字個數，內含 4 個整數個數、 3 個小數點數值的浮點數

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

