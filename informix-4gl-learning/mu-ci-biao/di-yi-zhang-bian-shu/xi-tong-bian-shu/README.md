---
description: Informix-4GL 系統變數使用說明
---

# SQLCA 系統變數

## SQLCA

系統內定總體變數  
Sructured Query Language Communication Access

```objectivec
DEFINE SQLCA RECORD
       SQLCODE INTEGER,
       SQLERRM CHAR(71),
       SQLERRP CHAR(8),
       SQLERRD ARRAY[6] OF INTEGER,
       SQLWARN CHAR(8)
END RECORD
```

1. [SQLCA.SQLCODE](sqlca.sqlcode.md)
2. [SQLCA.SQLERRM](sqlca.sqlerrm.md)
3. [SQLCA.SQLERRP](sqlca.sqlerrp.md)
4. [SQLCA.SQLERRD](sqlca.sqlerrd.md)
5. [SQLCA.SQLWARN](sqlca.sqlwarn.md)

{% hint style="danger" %}
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/45997552-informix-4gl-%e7%b3%bb%e7%b5%b1%e5%85%a7%e5%ae%9a%e7%b8%bd%e9%ab%94%e8%ae%8a%e6%95%b8%e3%80%8a-sqlca-%e3%80%8b) 】  
如有建議芒果改進的地方，請前往芒果留言區留言  
使芒果與你們一起成長進步
{% endhint %}

