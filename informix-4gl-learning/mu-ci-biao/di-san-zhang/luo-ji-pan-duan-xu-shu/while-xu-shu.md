---
description: Informix-4GL 循環迴圈敘述說明
---

# WHILE

```objectivec
WHILE booleanExpr
    ...
    [ CONTINUE WHILE ]
    ...
    [ EXIT WHILE ]
    ...
END WHILE
```

{% hint style="warning" %}
備註

booleanExpr  結果只能為  TRUE  或  FALSE  ，不能為  UNKNOWN  ，如結果為  TRUE  時，會開始執行  WHILE  敘述，反之，如結果為  FALSE  時，則離開  WHILE  敘述，並執行  END WHILE  敘述後面的程式\
CONTINUE WHILE  敘述會中斷程式，並執行下一次  WHILE  敘述  booleanExpr  判斷\
EXIT WHILE  敘述會結束  WHILE  敘述，並開始執行  END WHILE  敘述後面的程式\
END WHILE  敘述會重新執行  booleanExpr  判斷
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
