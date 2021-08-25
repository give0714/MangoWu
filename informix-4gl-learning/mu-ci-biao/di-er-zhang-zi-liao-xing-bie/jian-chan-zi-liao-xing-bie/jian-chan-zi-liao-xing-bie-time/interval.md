---
description: Informix-4GL 資料型別說明_TIME 資料型態
---

# INTERVAL

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
      <td style="text-align:left">INTERVAL largestTime(m) TO smallestTime(n)</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">m : &#x8A2D;&#x5B9A;&#x8A08;&#x7B97;&#x8D77;&#x59CB;&#x6642;&#x9593;&#x7684;&#x4F4D;&#x6578;</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">n : &#x8A2D;&#x5B9A;&#x8A08;&#x7B97;&#x7D50;&#x675F;&#x6642;&#x9593;&#x7684;&#x4F4D;&#x6578;</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x7FA4;&#x7D44;&#x4E00;</td>
      <td style="text-align:left">YEAR &#x3001; MONTH</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x7FA4;&#x7D44;&#x4E8C;</td>
      <td style="text-align:left">DAY &#x3001; HOUR &#x3001; MINUTE &#x3001; SECOND &#x3001;FRACTION</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x4F7F;&#x7528;&#x65B9;&#x6CD5;</td>
      <td style="text-align:left">
        <p>&#x7528;&#x65BC;&#x8A08;&#x7B97; DATE &#x3001;DATETIME &#x3001; INTERVAL
          &#x7684;&#x6642;&#x9593;&#x9593;&#x8DDD;</p>
        <p>&#x53EF;&#x6309;&#x4EFB;&#x4F55;&#x9806;&#x5E8F;&#x6392;&#x5217;</p>
        <p>&#x8A08;&#x7B97;&#x7D50;&#x679C;&#x70BA;&#x6B63;&#x503C;&#x6216;&#x8CA0;&#x503C;&#x7684;
          INTERVAL &#x8CC7;&#x6599;&#x578B;&#x5225;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8AAA;&#x660E;</td>
      <td style="text-align:left">&#x53EA;&#x80FD;&#x540C;&#x6642;&#x904B;&#x7528;&#x4E0A;&#x8FF0;&#x5176;&#x4E2D;&#x4E00;&#x7FA4;&#x7D44;</td>
    </tr>
  </tbody>
</table>

### 一、DATETIME 運算範例

#### 範例一之一

```objectivec
DEFINE timeInterval INTERVAL YEAR TO MONTH
...
LET timeInterval = DATETIME (2003-9) YEAR TO MONTH
                 - DATETIME (2003-8) YEAR TO MONTH
DISPLAY timeInterval

=>> 1
```

#### 範例一之一

```objectivec
DEFINE timeInterval INTERVAL YEAR TO MONTH
...
LET timeInterval = DATETIME (2005-09) YEAR TO MONTH
                 - DATETIME (2005-10) YEAR TO MONTH
DISPLAY timeInterval

=>> -1
```

#### 範例二之一

```objectivec
DEFINE timeInterval INTERVAL DAY TO SECOND
...
LET timeInterval = DATETIME (23 12:00:00) DAY TO SECOND
                 - DATETIME (14 12:30:00) DAY TO SECOND
DISPLAY timeInterval

=>> 8 23:30:00
```

#### 範例二之二

```objectivec
DEFINE timeInterval INTERVAL DAY TO SECOND
...
LET timeInterval = DATETIME (22 12:00:00) DAY TO SECOND
                 - DATETIME (22 12:30:00) DAY TO SECOND
DISPLAY timeInterval

=>> -30:00
```

### 二、DATE 運算範例

#### 範例一

```objectivec
DEFINE timeInterval INTERVAL YEAR TO YEAR
...
LET timeInterval = DATE ('2007-02-05') - DATE ('1968-06-04')
DISPLAY timeInterval 

=>> 39
```

#### 範例二

```objectivec
DEFINE timeInterval INTERVAL MONTH TO MONTH
...
LET timeInterval = DATE ('2007-02-05') - DATE ('2007-06-04')
DISPLAY timeInterval 

=>> -4
```

#### 範例三

```objectivec
DEFINE timeInterval INTERVAL DAY(5) TO DAY
...
LET timeInterval = (DATE ('2007/02/05') - DATE ('1968/06/04')) UNITS DAY
DISPLAY timeInterval

=>> 12810
```

#### 範例四

```objectivec
EXTEND (DATE ('5/2/2007'), YEAR TO MONTH) - DATE ('4/6/1969')

=>> INTERVAL (39-01) YEAR TO MONTH
```

### 三、INTERVAL 運算範例

#### 範例一

```objectivec
DEFINE timeInterval INTERVAL MINUTE(3) TO FRACTION(4)
...
LET timeInterval = INTERVAL (100:30.0005) MINUTE(3) TO FRACTION(4)
                 - INTERVAL (120.01) SECOND(3) TO FRACTION
DISPLAY timeInterval

=>> 98:29.9905
```

#### 範例二

```objectivec
DEFINE timeInterval INTERVAL MINUTE TO FRACTION(4)
...
LET timeInterval = INTERVAL (15:30.0002) MINUTE TO FRACTION(4) * 2.5
DISPLAY timeInterval

=>> 38:45.0005
```

### 四、組合運算

#### 範例一

```objectivec
DEFINE timeInterval DATETIME YEAR TO DAY
...
LET timeInterval = DATETIME (2000-8-1) YEAR TO DAY
                 + INTERVAL (3-5) YEAR TO MONTH
DISPLAY timeInterval

=>> 2004-01-01
```

#### 範例二

```objectivec
DEFINE timeInterval DATETIME YEAR TO MINUTE
...
LET timeInterval = EXTEND ( DATETIME (2008-8-1) YEAR TO DAY, YEAR TO MINUTE )
                 - INTERVAL (720) MINUTE(3) TO MINUTE
DISPLAY timeInterval

=>> 2008-07-31 12:00
```

說明：從加減 DATE 、 DATETIME 、 INTERVAL 資料型別的變數，按任何順序排列，可得到結果正值或負值的 INTERVAL 資料型別的變數

參考來源 : [IBM](https://www.ibm.com/docs/en/informix-servers/14.10?topic=bidt-time-data-types)

{% hint style="danger" %}
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/46114972-informix-4gl-%E7%B0%A1%E5%96%AE%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-time-data-%E3%80%8B%28-%E4%B8%89-%29) 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}



