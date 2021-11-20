---
description: Informix-4GL 系統變數使用說明
---

# SQLCA 系統變數

## SQLCA

系統內定總體變數\
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
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/45997552-informix-4gl-%E7%B3%BB%E7%B5%B1%E5%85%A7%E5%AE%9A%E7%B8%BD%E9%AB%94%E8%AE%8A%E6%95%B8%E3%80%8A-sqlca-%E3%80%8B) 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
