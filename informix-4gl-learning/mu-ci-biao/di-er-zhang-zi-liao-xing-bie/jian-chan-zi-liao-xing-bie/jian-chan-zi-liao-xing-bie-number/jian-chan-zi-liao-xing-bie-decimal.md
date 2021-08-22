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
      <td style="text-align:left">byte = ROUND ( precision / 2 + 1 )</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8CC7;&#x6599;&#x7BC4;&#x570D;</td>
      <td style="text-align:left">32&#x500B;&#x6578;&#x5B57;&#x500B;&#x6578;</td>
    </tr>
  </tbody>
</table>

#### 範例一

```objectivec
DEFINE unitPrice DECIMAL( 6 )
...
LET unitPrice = 11.0014
```

說明 : unitPrice 為有6個數字個數的浮點數

#### 範例二

```objectivec
DEFINE unitPrice DECIMAL( 6, 2 )
...
LET unitPrice = 4211.01
```

說明 : unitPrice 為有6個數字個數，內含4個整數個數、2個小數點數值的浮點數

