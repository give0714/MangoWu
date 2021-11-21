---
description: Informix-4GL 資料操作_SQL Language
---

# 新增語法

## 語法

```
INSERT INTO tableName [ columnName1 [, columnName2, ...]]
            VALUES( valueName1, [ valueName2, ...])
```

{% hint style="info" %}
功能：

新增資料至資料表內。
{% endhint %}

{% hint style="info" %}
說明：

IN dbspaceName：若省略不寫，該資料庫將會建立在 Informix Database Server 的 root dbspace 上。

WITH \[( BUFFERED / LOG MODE ANSI )] LOG ]：若省略不寫，則該資料庫就不會產生 log，後續將無法使用 Transaction 的語法。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
