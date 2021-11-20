---
description: Informix-4GL 資料型別說明_TIME 資料型態
---

# DATETIME

#### 說明

| 語法   | DATETIME ( dateTime ) beginDateTime TO endDateTime                                                                                                                                                                                                                                                                                             |
| ---- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|      | DATETIME beginDateTime TO endDateTime                                                                                                                                                                                                                                                                                                          |
| 資料長度 | 4 byte                                                                                                                                                                                                                                                                                                                                         |
| 範圍   | <p>YEAR            0001 ~9999</p><p>MONTH        01 ~ 12</p><p>DAY               01 ~ 31</p><p>HOUR            01 ~ 24</p><p>MINUTE        00 ~ 59</p><p>SECOND       00~59</p><p>FRACTION    00000 ~ 99999</p>                                                                                                                                |
| 格式   | yyyy/mm/dd hh:mm:ss.fffff ( n )                                                                                                                                                                                                                                                                                                                |
| 說明   | <p>可使用 / 、 . 、 - 做分隔</p><p>year 為四位數，介於 0000 到 9999 之間<br>若只輸入兩位數，則預設為 19XX</p><p>如需使用民國年份，且系統為 UNIX 的 Bournel shell ，<br>可再 .profile 檔設定 DBDATE = Y2MD/;</p><p>                                    export DBDATE;</p><p>month 和 day 為兩位數，可補 0 或不補 0</p><p>hour、minute 、 second 為兩位數，介於 00 到 59 之間</p><p>fraction 為五位數，介於 00000 到 99999 之間</p> |

#### 範例一

```objectivec
DEFINE birthday DATETIME YEAR TO FRACTION
...
LET birthday = '2021-08-22 12:01:00.00001'
DISPLAY birthday

=>> 2021-08-22 12:01:00.00001
```

#### 範例二

```objectivec
DEFINE birthday DATETIME YEAR TO DAY
...
LET birthday = '2021-08-22'
DISPLAY birthday

=>> 2021-08-22
```

#### 範例二

```objectivec
DEFINE birthday DATETIME HOUR TO SECOND
...
LET birthday = '12:30:01'
DISPLAY birthday

=>> 12:30:01
```

{% hint style="danger" %}
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/46113376-informix-4gl-%E7%B0%A1%E5%96%AE%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-time-data-%E3%80%8B\(-%E4%BA%8C-\)) 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
