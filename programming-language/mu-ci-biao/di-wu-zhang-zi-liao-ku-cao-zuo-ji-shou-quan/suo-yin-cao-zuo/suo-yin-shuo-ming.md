---
description: Informix-4GL 索引操作
---

# 索引說明

{% hint style="info" %}
索引種類：

單行索引 Single - Column Indexes

&#x20;              僅使用單行做索引

多行索引 Multiple - Column Indexes

&#x20;              使用一個以上的行做索引
{% endhint %}

{% hint style="info" %}
索引說明：

為含有索引的行值，會記錄索引碼〈指標值 Point〉
{% endhint %}

{% hint style="info" %}
索引使用時機：

用以連結〈JOIN〉兩個表以上的行值。

無法建立含有大量重複值的行，一個行不能超過65536的重複值。

一個表不能有8個以上的索引。

無法將120位元組以上長度的行，建立做為索引
{% endhint %}

{% hint style="info" %}
升冪 & 降冪：

預設索引為升冪排序。

排序方式：

1. 字元 CHAR【A \~ Z】
2. 數值和錢值【小\~大】
3. 日期 DATE【依年份由小 \~ 大】

語法：

```
CREATE INDEX indexName ON tableName
     ( columnName1 datatype [( DESC / ASC )],
       [ columnName2 datatype [( DESC / ASC )], ...])
```
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
