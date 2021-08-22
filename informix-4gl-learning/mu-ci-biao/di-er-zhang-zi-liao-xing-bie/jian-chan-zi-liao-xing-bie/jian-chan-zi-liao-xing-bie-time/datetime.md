---
description: Informix-4GL 資料型別說明_TIME 資料型態
---

# DATETIME

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
      <td style="text-align:left">DATETIME ( dateTime ) beginDateTime TO endDateTime</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8CC7;&#x6599;&#x9577;&#x5EA6;</td>
      <td style="text-align:left">4 byte</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x683C;&#x5F0F;</td>
      <td style="text-align:left">yyyy/mm/dd hh:mm:ss.fffff</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8AAA;&#x660E;</td>
      <td style="text-align:left">
        <p>&#x53EF;&#x4F7F;&#x7528; / &#x3001; . &#x3001; - &#x505A;&#x5206;&#x9694;</p>
        <p>year &#x70BA;&#x56DB;&#x4F4D;&#x6578;&#xFF0C;&#x4ECB;&#x65BC; 0000 &#x5230;
          9999 &#x4E4B;&#x9593;
          <br />&#x82E5;&#x53EA;&#x8F38;&#x5165;&#x5169;&#x4F4D;&#x6578;&#xFF0C;&#x5247;&#x9810;&#x8A2D;&#x70BA;
          19XX</p>
        <p>&#x5982;&#x9700;&#x4F7F;&#x7528;&#x6C11;&#x570B;&#x5E74;&#x4EFD;&#xFF0C;&#x4E14;&#x7CFB;&#x7D71;&#x70BA;
          UNIX &#x7684; Bournel shell &#xFF0C;
          <br />&#x53EF;&#x518D; .profile &#x6A94;&#x8A2D;&#x5B9A; DBDATE = Y2MD/;</p>
        <p>export DBDATE;</p>
        <p>month &#x548C; day &#x70BA;&#x5169;&#x4F4D;&#x6578;&#xFF0C;&#x53EF;&#x88DC;
          0 &#x6216;&#x4E0D;&#x88DC; 0</p>
        <p>hour&#x3001;minute &#x3001; second &#x70BA;&#x5169;&#x4F4D;&#x6578;&#xFF0C;&#x4ECB;&#x65BC;
          00 &#x5230; 59 &#x4E4B;&#x9593;</p>
        <p>fraction &#x70BA;&#x4E94;&#x4F4D;&#x6578;&#xFF0C;&#x4ECB;&#x65BC; 00000
          &#x5230; 99999 &#x4E4B;&#x9593;</p>
      </td>
    </tr>
  </tbody>
</table>

#### 範例一

```objectivec
DEFINE birthday DATETIME
...
LET birthday = '2021-08-22 12:01:00.00001'
```

