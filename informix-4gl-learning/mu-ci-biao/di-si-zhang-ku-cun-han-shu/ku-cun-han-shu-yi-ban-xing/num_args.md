---
description: Informix-4GL 庫存函數_一般型使用說明
---

# NUM_ARGS( )

## 語法一

```
NUM_ARGS( )
```

## 語法二

```
ARG_VAL( NUM_ARGS( ) )
```

### 範例

```
// EX：在命令列打入-【rogramName.4ge "ABC" "XYZ"】
// 傳入兩個參數
DEFINE f_a                  CHAR(20)

LET f_a = ARG_VAL(1)
DISPLAY "命令列第一個傳入的資料為 ", f_a

LET f_a = ARG_VAL(2)
DISPLAY "命令列第二個傳入的資料為 ", f_a

LET f_a = ARG_VAL(0)
DISPLAY "程式名稱為 ", f_a

=>> 命令列第一個傳入的資料為 ABC
=>> 命令列第二個傳入的資料為 XYZ
=>> 程式名稱為 XXX
```

{% hint style="info" %}
目的：

傳回命令列之傳入的參數總數量
{% endhint %}

{% hint style="info" %}
說明：

需搭配 ARG_VAL( ) 使用
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】\
如有建議芒果改進的地方，請前往芒果留言區留言\
使芒果與你們一起成長進步
{% endhint %}
