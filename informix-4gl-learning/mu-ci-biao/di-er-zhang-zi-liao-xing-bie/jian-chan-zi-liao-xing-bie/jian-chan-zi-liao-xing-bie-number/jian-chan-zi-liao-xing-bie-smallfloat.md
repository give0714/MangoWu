---
description: Informix-4GL 資料型別說明_Number 資料型態
---

# SMALLFLOAT

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
      <td style="text-align:left">SMALLFLOAT</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8CC7;&#x6599;&#x9577;&#x5EA6;</td>
      <td style="text-align:left">4 byte</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x5225;&#x540D;</td>
      <td style="text-align:left">
        <p>1.&#x55AE;&#x7CBE;&#x6E96;&#x6D6E;&#x9EDE;&#x6578;</p>
        <p>2.&#x5BE6;&#x6578; &lt; REAL &gt;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8AAA;&#x660E;</td>
      <td style="text-align:left">&#x76F8;&#x7576;&#x70BA; C &#x8A9E;&#x8A00;&#x7684; FLOAT &#x8CC7;&#x6599;&#x578B;&#x5225;</td>
    </tr>
  </tbody>
</table>

#### 範例一

```objectivec
DEFINE sf SMALLFLOAT
...
LET sf = 11.01

=>> $ 11.01
```

#### 範例二

```objectivec
DEFINE sf SMALLFLOAT
...
LET sf = 

=>> $ 11.01
```

{% hint style="warning" %}
強烈建議將 SMALLFLOAT 資料型別改使用成 DECIMAL 資料型別
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

