---
description: Informix-4GL 資料操作_游標種類
---

# 游標種類

## Scrolling CURSOR

* 常用於查詢功能方面。
* 可前或後移動 CURSOR。

## Non-Scrolling CURSOR

* 常用於報表功能方面。
* 僅能向後移動 CURSOR 游標。

## For Update CURSOR

* 常用於資料修改或資料刪除。
* 僅能向後移動 CURSOR 游標。
* 會將 CURSOR 游標指到的資料鎖定，直到 CURSOR 游標移動置其他資料，才會將其解鎖。
* 又稱為 Locking CURSOR。



{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
