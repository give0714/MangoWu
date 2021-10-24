---
description: Informix-4GL 資料型別說明_Number 資料型態
---

# MONEY

#### 說明

| 語法   | MONEY ( precision \[, scale ] )    |
| ---- | ---------------------------------- |
|      | precision : 所有數字個數，不含小數點，預設為 16    |
|      | scale : 所有小數點右邊的數字個數，預設為 2         |
| 資料長度 | byte = ROUND ( precision / 2 + 1 ) |
| 資料範圍 | 32個數字個數                            |
| 說明   | 系統自動帶入錢制符號 $ ，預設以浮點數型態表示           |

#### 範例一

```objectivec
DEFINE unitPrice MONEY
...
LET unitPrice = 1048.145
DISPLAY unitPrice

=>> $ 1048.14
```

說明 : unitPrice 為預設 16 個數字個數的浮點數，內含 2 個小數點數值的浮點數

#### 範例二

```objectivec
DEFINE unitPrice MONEY( 6 )
...
LET unitPrice = 11.0114
DISPLAY unitPrice

=>> $ 11.01
```

說明 : unitPrice 為有6個數字個數的浮點數

#### 範例三

```objectivec
DEFINE unitPrice MONEY( 6, 2 )
...
LET unitPrice = 4211.01
DISPLAY unitPrice

=>> $ 4211.01
```

說明 : unitPrice 為有6個數字個數，內含4個整數個數、2個小數點數值的浮點數

{% hint style="danger" %}
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/46111630-informix-4gl-%E7%B0%A1%E5%96%AE%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-numeric-data-%E3%80%8B\(-%E4%B8%83-\)) 】\
如有建議芒果改進的地方，請前往芒果留言區留言\
使芒果與你們一起成長進步
{% endhint %}
