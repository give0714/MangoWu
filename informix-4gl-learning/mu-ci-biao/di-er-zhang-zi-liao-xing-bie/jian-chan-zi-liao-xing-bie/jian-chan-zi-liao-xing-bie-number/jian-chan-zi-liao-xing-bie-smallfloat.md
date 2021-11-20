---
description: Informix-4GL 資料型別說明_Number 資料型態
---

# SMALLFLOAT

#### 說明

| 語法   | SMALLFLOAT                               |
| ---- | ---------------------------------------- |
| 資料長度 | 4 byte                                   |
| 別名   | <p>1.單精準浮點數</p><p>2.實數 &#x3C; REAL ></p> |
| 說明   | 相當為 C 語言的 FLOAT 資料型別                     |

#### 範例一

```objectivec
DEFINE sf SMALLFLOAT
...
LET sf = 11.01
DISPLAY sf

=>> 11.01
```

#### 範例二

```objectivec
DEFINE sf SMALLFLOAT
...
LET sf = 89.4128
DISPLAY sf

=>> 89.41
```

{% hint style="warning" %}
強烈建議將 SMALLFLOAT 資料型別改使用成 DECIMAL 資料型別
{% endhint %}

{% hint style="danger" %}
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/46111225-informix-4gl-%E7%B0%A1%E5%96%AE%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-numeric-data-%E3%80%8B\(-%E4%BA%94-\)) 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
