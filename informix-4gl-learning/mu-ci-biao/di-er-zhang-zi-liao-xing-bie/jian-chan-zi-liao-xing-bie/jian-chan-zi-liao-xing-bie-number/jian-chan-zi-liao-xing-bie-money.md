---
description: Informix-4GL 資料型別說明_Number 資料型態
---

# MONEY

#### 說明

|  |  |
| :--- | :--- |
| 語法 | MONEY \( precision \[, scale \] \) |
|  | precision : 所有數字個數，不含小數點，預設為 16 |
|  | scale : 所有小數點右邊的數字個數，預設為 2 |
| 資料長度 | byte = ROUND \( precision / 2 + 1 \) |
| 資料範圍 | 32個數字個數 |
| 說明 | 系統自動帶入錢制符號 $ ，預設以浮點數型態表示 |

#### 範例一

```objectivec
DEFINE unitPrice MONEY( 6 )
...
LET unitPrice = 11.0014

=>> $11.0014
```

說明 : unitPrice 為有6個數字個數的浮點數

#### 範例二

```objectivec
DEFINE unitPrice MONEY( 6, 2 )
...
LET unitPrice = 4211.01

=>> $4211.01
```

說明 : unitPrice 為有6個數字個數，內含4個整數個數、2個小數點數值的浮點數

