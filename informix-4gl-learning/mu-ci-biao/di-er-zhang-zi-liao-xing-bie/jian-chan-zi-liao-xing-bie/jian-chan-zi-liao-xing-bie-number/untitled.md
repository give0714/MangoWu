---
description: Informix-4GL 資料型別說明_Number 資料型態
---

# FLOAT

#### 說明

|  |  |
| :--- | :--- |
| 語法 | FLOAT |
| 資料長度 | 8 byte |
| 別名 | 倍精準浮點數 |
| 說明 | 相當為 C 語言的 DOUBLE 資料型別 |

#### 範例一

```objectivec
DEFINE f FLOAT
...
LET f = 11.0214
DISPLAY f

=>> 11.02
```

#### 範例二

```objectivec
DEFINE f FLOAT
...
LET f = 89.4128
DISPLAY f

=>> 89.41
```

{% hint style="warning" %}
強烈建議將 FLOAT 資料型別改使用成 DECIMAL 資料型別
{% endhint %}

{% hint style="danger" %}
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/46111474-informix-4gl-%E7%B0%A1%E5%96%AE%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-numeric-data-%E3%80%8B%28-%E5%85%AD-%29) 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

