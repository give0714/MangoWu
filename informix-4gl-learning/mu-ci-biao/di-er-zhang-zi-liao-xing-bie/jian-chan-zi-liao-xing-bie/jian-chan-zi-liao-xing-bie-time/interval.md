---
description: Informix-4GL 資料型別說明_TIME 資料型態
---

# INTERVAL

#### 說明

| 語法   | INTERVAL largestTime(m) TO smallestTime(n)                                                 |
| ---- | ------------------------------------------------------------------------------------------ |
|      | m : 設定計算起始時間的位數                                                                            |
|      | n  : 設定計算結束時間的小數點位數，僅適用於 FRACTION                                                          |
| 群組一  | YEAR 、 MONTH                                                                               |
| 群組二  | DAY 、 HOUR 、 MINUTE 、 SECOND 、FRACTION                                                     |
| 使用方法 | <p>用於計算 DATE 、DATETIME 、 INTERVAL 的時間間距</p><p>可按任何順序排列</p><p>計算結果為正值或負值的 INTERVAL 資料型別</p> |
| 注意事項 | 只能同時運用上述其中一群組                                                                              |

### 一、DATETIME 運算範例

#### 範例一之一

```objectivec
DEFINE timeInterval INTERVAL YEAR TO MONTH
...
LET timeInterval = DATETIME (2003-9) YEAR TO MONTH
                 - DATETIME (2003-8) YEAR TO MONTH
DISPLAY timeInterval

=>> 0-01
```

#### 範例一之二

```objectivec
DEFINE timeInterval INTERVAL YEAR TO MONTH
...
LET timeInterval = DATETIME (2005-09) YEAR TO MONTH
                 - DATETIME (2005-10) YEAR TO MONTH
DISPLAY timeInterval

=>> -0-01
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

=>> -0 00:30:00
```

### 二、DATE 運算範例

#### 範例一

```objectivec
DEFINE timeInterval INTERVAL YEAR TO YEAR
...
LET timeInterval = EXTEND ( DATE ('2007-02-05'), YEAR TO YEAR )
                 - DATE ('1968-06-04')
DISPLAY timeInterval 

=>> 39
```

#### 範例二

```objectivec
DEFINE timeInterval INTERVAL MONTH TO MONTH
...
LET timeInterval = EXTEND ( DATE ('2007-02-05'), MONTH TO MONTH )
                 - DATE ('2007-06-04')
DISPLAY timeInterval 

=>> -4
```

#### 範例三

```objectivec
DEFINE timeInterval INTERVAL DAY(5) TO DAY
...
LET timeInterval = ( DATE ('2007/02/05') - DATE ('1968/06/04') ) UNITS DAY
DISPLAY timeInterval

=>> 14125
```

#### 範例四

```objectivec
DEFINE timeInterval INTERVAL YEAR TO MONTH
...
LET timeInterval = EXTEND ( DATE ('2007-02-05'), YEAR TO MONTH )
                 - DATE ('1969-06-04')
DISPLAY timeInterval

=>> 37-08
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

參考來源 : [IBM](https://www.ibm.com/docs/en/informix-servers/14.10?topic=bidt-time-data-types)

{% hint style="danger" %}
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/46114972-informix-4gl-%E7%B0%A1%E5%96%AE%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-time-data-%E3%80%8B\(-%E4%B8%89-\)) 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}

