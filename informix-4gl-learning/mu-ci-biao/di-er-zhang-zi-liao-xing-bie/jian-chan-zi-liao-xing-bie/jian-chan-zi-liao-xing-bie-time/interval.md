---
description: Informix-4GL 資料型別說明_TIME 資料型態
---

# INTERVAL

#### 說明

|  |  |
| :--- | :--- |
| 語法 | INTERVAL \( dateTime \) largestTime\(m\) TO smallestTime\(n\) |
| 群組一 | YEAR 、 MONTH |
| 群組二 | DAY 、 HOUR 、 MINUTE 、 SECOND 、FRACTION |
| 使用方法 | 用於計算 DATE 、DATETIME 、 INTERVAL 的時間間距，可按任何順序排列，結果為正值或負值的 INTERVAL 資料型別 |
| 說明 | 同時只能使用其中一群組 |

#### 範例一

```objectivec
DATETIME (2003-9-30 12:30) YEAR TO MINUTE
- DATETIME (2003-8-1 11:00) YEAR TO HOUR

Result: INTERVAL (60 01:30) DAY TO MINUTE
```

#### 範例二

```objectivec
DATETIME (2005-9-30) YEAR TO DAY
- DATETIME (2005-10-1) MONTH TO DAY

Result: INTERVAL (-1) DAY TO DAY
```

#### 範例三

```objectivec
DATETIME (2000-8-1) YEAR TO DAY
+ INTERVAL (3-5) YEAR TO MONTH

Result: DATETIME (2004-01-01) YEAR TO DAY
```

#### 範例四

```objectivec
EXTEND (DATETIME (2008-8-1) YEAR TO DAY, YEAR TO MINUTE)
   - INTERVAL (720) MINUTE(3) TO MINUTE

Result: DATETIME (2008-07-31 12:00) YEAR TO MINUTE
```

#### 範例五

```objectivec
(DATE ('5/2/2007') - DATE ('4/6/1968')) UNITS DAY

Result: INTERVAL (12810) DAY(5) TO DAY
```

#### 範例六

```objectivec
EXTEND (DATE ('5/2/2007'), YEAR TO MONTH) - DATE ('4/6/1969')

Result: INTERVAL (39-01) YEAR TO MONTH
```

#### 範例七

```objectivec
INTERVAL (100:30.0005) MINUTE(3) TO FRACTION(4)
   - INTERVAL (120.01) SECOND(3) TO FRACTION

Result: INTERVAL (98:29.9905) MINUTE TO FRACTION(4)
```

#### 範例八

```objectivec
INTERVAL (15:30.0002) MINUTE TO FRACTION(4) * 2.5

Result: INTERVAL (38:45.0005) MINUTE TO FRACTION(4)
```

說明：從加減 DATE 、 DATETIME 、 INTERVAL 資料型別的變數，按任何順序排列，可得到結果正值或負值的 INTERVAL 資料型別的變數

參考來源 : [IBM](https://www.ibm.com/docs/en/informix-servers/14.10?topic=bidt-time-data-types)

