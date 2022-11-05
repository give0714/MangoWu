---
description: Informix-4GL 畫面操作說明
---

# ATTRIBUTE 語法

## 語法

```inform7
ATTRIBUTE ( [ ( BLACK / BLUE / CYAN / GREEN / MAGENTA / RED / WHILE / YELLOW ) ]
            [ ( BOLD / DIM / INVISIBLE / NORMAL ) ]
            [ ( REVERSE / BLINK / UNDERLINE ) ]
            [ CURREN ROW DISPLAY = "特效, ..." ]              -- 限 INPUT ARRAY 敘述使用 --
            [ COUNT              = ( int / variableName ) ]   -- 限 INPUT ARRAY 敘述使用 --
            [ MAXCOUNT           = ( int / variableName ) ]   -- 限 INPUT ARRAY 敘述使用 --
            [ INSERT ROW         = ( TRUE / FALSE ) ]         -- 限 INPUT ARRAY 敘述使用 --
            [ DELETE ROW         = ( TRUE / FALSE ) ] )       -- 限 INPUT ARRAY 敘述使用 --
```

{% hint style="info" %}
使用地方：

1. CONSTRUCT 敘述
2. DISPLAY FORM 敘述
3. DISPLAY ARRAY 敘述
4. DISPLAY TO 敘述
5. DISPLAY AT 敘述
6. DISPLAY BY NAME 敘述
7. INPUT 敘述
8. INPUT ARRAY 敘述
9. MESSAGE 敘述
10. ERROR 敘述
11. PROMPT 敘述
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
