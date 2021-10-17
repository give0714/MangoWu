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

LET f_a = NUM_AGES( )
DISPLAY "命令列共傳入 ", f_a USING "&", "筆資料"

=>> 命令列共傳入 2 筆資料
```

{% hint style="info" %}
目的：

傳回命令列之傳入的參數總數量。
{% endhint %}

{% hint style="info" %}
說明：

需搭配 ARG_VAL( ) 使用。
{% endhint %}

{% hint style="danger" %}
前往【 城市芒果留言區 】\
如有建議芒果改進的地方，請前往芒果留言區留言\
使芒果與你們一起成長進步
{% endhint %}
