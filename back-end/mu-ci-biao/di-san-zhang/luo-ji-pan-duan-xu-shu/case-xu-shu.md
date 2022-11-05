---
description: Informix-4GL 條件選擇敘述說明
---

# CASE

```objectivec
CASE
     WHEN selector = expression
          ...
          [ EXIT CASE ]
     ...
     OTHERWISE
               ...
END CASE
```

{% hint style="warning" %}
備註

selector = expression  結果只能為  TRUE  或  FALSE  ，不能為  UNKNOWN  ，如結果為  TRUE  時，會開始執行該  WHEN  敘述，執行到，反之  EXIT CASE  敘述時，會結束整個  CASE  敘述，並執行  END CASE 敘述後面的程式，如結果為  FALSE  時，則會繼續後續  WHEN  敘述判斷，一直到全部  WHEN  敘述都判斷完畢，且同時無執行任一  WHEN  敘述時，則會執行  OTHERWISE  敘述的程式，執行結束後，才會執行  END CASE 敘述後面的程式
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
