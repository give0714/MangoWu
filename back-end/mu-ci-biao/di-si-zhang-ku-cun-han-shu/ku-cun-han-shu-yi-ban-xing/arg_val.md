---
description: Informix-4GL 庫存函數_一般型使用說明
---

# ARG\_VAL( )

## 語法

```
AGE_VAL( num )
```

{% hint style="info" %}
目的：

可在編寫執行程式之名稱後面加上欲傳入的值，並傳回 CHAR 的命令列參數。
{% endhint %}

{% hint style="info" %}
說明：

可搭配 NUM\_ARGS( ) 使用，用以從命令列傳遞資料至程式，可回傳命令列的參數數目。

expr ：整數表示式，介於 0 \~ NUM\_ARGS( ) 之間。

ARG\_VAL( 0 ) ：自身的程式名稱。
{% endhint %}

### 範例一

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

### 範例二

```
// EX：在命令列打入-【rogramName.4ge "ABC"】
// 傳入一個參數
DEFINE f_a                  CHAR(20)

LET f_a = ARG_VAL(1)
DISPLAY "命令列第一個傳入的資料為 ", f_a

LET f_a = ARG_VAL(2)
DISPLAY "命令列第二個傳入的資料為 ", f_a

LET f_a = ARG_VAL(0)
DISPLAY "程式名稱為 ", f_a

=>> 命令列第一個傳入的資料為 ABC
=>> 命令列第二個傳入的資料為
=>> 程式名稱為 XXX
```

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
