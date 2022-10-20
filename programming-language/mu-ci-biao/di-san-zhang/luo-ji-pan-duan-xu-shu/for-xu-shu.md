---
description: Informix-4GL 固定迴圈敘述說明
---

# FOR

```objectivec
FOR variable = integerExpr TO integerExpr [ STEP integer ]
    ...
    [ CONTINUE FOR ]
    ...
    [ EXIT FOR ]
    ...
END FOR
```

{% hint style="warning" %}
備註

variable  為程式變數，或是  datatype  為  SMALLINT  或  INTEGER  的數值，需先宣告\
integerExpr  為  SMALLINT  或  INTEGER  的  datatype  表示式\
CONTINUE FOR  敘述會中斷程式，並執行下一次  FOR  敘述\
EXIT FOR  敘述會結束  FOR  敘述，並開始執行  END FOR  敘述後面的程式\
END FOR  敘述預設於第一次判斷過後，每次執行判斷前先行加一
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
