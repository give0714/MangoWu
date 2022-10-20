---
description: Informix-4GL 資料型別說明_Number 資料型態
---

# DECIMAL

#### 說明

| 語法   | DECIMAL ( precision \[, scale ] )                                                                                                                                                                                                               |
| ---- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|      | precision : 所有數字個數，不含小數點，預設為 16                                                                                                                                                                                                                 |
|      | <p>scale : 所有小數點右邊的數字個數</p><p>             預設範圍 10(-128) ~ 10(126)</p>                                                                                                                                                                          |
| 資料長度 | <p>byte = ROUND ( precision / 2 + 1 )</p><p>1.DECIMAL ( precision )</p><p>    1+ precision / 2  byte</p><p>2.DECIMAL ( precision [, scale ] )</p><p>   scale 為奇數 ( precision + 3 ) / 2  byte</p><p>   scale 為偶數 ( precision + 4 ) / 2  byte</p> |
| 資料範圍 | 32個數字個數                                                                                                                                                                                                                                         |

#### 範例一

```objectivec
DEFINE unitPrice DECIMAL
...
LET unitPrice = 1048.14
DISPLAY unitPrice

=>> 1048.14
```

說明 : unitPrice 為預設 16 個數字個數的浮點數，內含 2 個小數點數值的浮點數

#### 範例二

```objectivec
DEFINE unitPrice DECIMAL( 9 )
...
LET unitPrice = 8791211.14
DISPLAY unitPrice

=>> 8791211.14
```

說明 : unitPrice 為有 9 個數字個數的浮點數

#### 範例三

```objectivec
DEFINE unitPrice DECIMAL( 7, 3 )
...
LET unitPrice = 4211.012
DISPLAY unitPrice

=>> 4211.012
```

說明 : unitPrice 為有 7 個數字個數，內含 4 個整數個數、 3 個小數點數值的浮點數

{% hint style="danger" %}
【 [M@nGo 留言區](https://give0714.pixnet.net/blog/post/46110625-informix-4gl-%E7%B0%A1%E5%96%AE%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-numeric-data-%E3%80%8B\(-%E5%9B%9B-\)) 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
