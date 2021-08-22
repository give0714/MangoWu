---
description: Informix-4GL 資料型別說明_SERIAL 資料型態
---

# SERIAL

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
      <td style="text-align:left">SERIAL</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">SERIAL( n )</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8CC7;&#x6599;&#x9577;&#x5EA6;</td>
      <td style="text-align:left">4 byte</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8CC7;&#x6599;&#x7BC4;&#x570D;</td>
      <td style="text-align:left">1 ~ 2147483647</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8AAA;&#x660E;</td>
      <td style="text-align:left">
        <p>1.&#x6BCF;&#x4E00;&#x8CC7;&#x6599;&#x8868;&#x53EA;&#x6709;&#x4E00;&#x500B;
          SERIAL &#xFF0C;&#x8A2D;&#x5B9A;&#x5F8C;&#x7121;&#x6CD5;&#x6539;&#x8B8A;&#x5E8F;&#x865F;</p>
        <p>2.&#x82E5;&#x5E8F;&#x865F;&#x88AB;&#x522A;&#x9664;&#xFF0C;&#x5247;&#x6B64;&#x522A;&#x9664;&#x5E8F;&#x865F;&#x865F;&#x78BC;&#x5C07;&#x7121;&#x6CD5;&#x88AB;&#x4F7F;&#x7528;</p>
        <p>3.&#x65B0;&#x589E;&#x8CC7;&#x6599;&#x6642;&#xFF0C;&#x7CFB;&#x7D71;&#x6703;&#x81EA;&#x52D5;&#x7D2F;&#x52A0;&#x65B0;&#x589E;&#x865F;&#x78BC;</p>
      </td>
    </tr>
  </tbody>
</table>

#### 範例一

```objectivec
DEFINE employeeNum SERIAL
```

說明： employeeNum 起始值為 1 ，後續新增資料會以此累加 1

#### 範例二

```objectivec
DEFINE employeeNum SERIAL(1001)
```

說明： employeeNum 起始值為 1001 ，後續新增資料會以此累加 1

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

