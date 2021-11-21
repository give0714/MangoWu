---
description: Informix-4GL SQLCODE 變數說明
---

# SQLCA.SQLCODE

| SQLCODE 狀態          | 說明                        |
| ------------------- | ------------------------- |
| SQLCA.SQLCODE = 0   | 表示 SQL 執行成功               |
| SQLCA.SQLCODE = 100 | 表示 SQL 執行成功，但未有符合條件的資料被取出 |
| SQLCA.SQLCODE < 0   | 表示 SQL 執行失敗               |

{% hint style="info" %}
#### 說明

反映 SQL 指令執行後的結果
{% endhint %}

{% hint style="danger" %}
【 [M@nGo 留言區](https://give0714.pixnet.net/blog/post/45999613-informix-4gl-%E7%B3%BB%E7%B5%B1%E5%85%A7%E5%AE%9A%E7%B8%BD%E9%AB%94%E8%AE%8A%E6%95%B8-sqlca-\(-%E4%BA%8C-\)) 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
