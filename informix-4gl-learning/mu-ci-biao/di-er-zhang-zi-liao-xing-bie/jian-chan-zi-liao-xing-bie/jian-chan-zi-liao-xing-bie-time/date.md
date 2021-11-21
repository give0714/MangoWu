---
description: Informix-4GL 資料型別說明_TIME 資料型態
---

# DATE

#### 說明

| 語法   | DATE                                                                                                                                                                                                                                                     |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 資料長度 | 4 byte                                                                                                                                                                                                                                                   |
| 格式   | <p>yyyy-mm-dd  ||  yyyy/mm/dd  ||  yyyy.mm.dd</p><p>yy-mm-dd      ||  yy/mm/dd      ||  yy.mm.dd</p>                                                                                                                                                     |
| 說明   | <p>可使用 / 、 . 、 - 做分隔</p><p>year 為四位數，介於 0000 到 9999 之間<br>若只輸入兩位數，則預設為 19XX</p><p>如需使用民國年份，且系統為 UNIX 的 Bournel shell ，<br>可再 .profile 檔設定 DBDATE = Y2MD/;</p><p>                                    export DBDATE;</p><p>month 和 day 為兩位數，可補 0 或不補 0</p> |

#### 範例一

```objectivec
DEFINE birthday DATE
...
LET birthday = '2021/08/22'
DISPLAY birthday

=>> 2021/08/22
```

#### 範例二

```objectivec
DEFINE birthday DATE
...
LET birthday = '2021-08-22'
DISPLAY birthday

=>> 2021/08/22
```

#### 範例三

```objectivec
DEFINE birthday DATE
...
LET birthday = '2021.08.22'
DISPLAY birthday

=>> 2021/08/22
```

{% hint style="danger" %}
【 [M@nGo 留言區](https://give0714.pixnet.net/blog/post/46112041-informix-4gl-%E7%B0%A1%E5%96%AE%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-time-data-%E3%80%8B\(-%E4%BA%8C-\)) 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
