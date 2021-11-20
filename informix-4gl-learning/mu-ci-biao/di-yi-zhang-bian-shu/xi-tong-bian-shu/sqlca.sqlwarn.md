---
description: Informix-4GL SQLWARN 變數說明
---

# SQLCA.SQLWARN

| SQLWARN 狀態           | 說明                                                                                              |
| -------------------- | ----------------------------------------------------------------------------------------------- |
| SQLCA.SQLWARN \[ 1 ] | <p>當 [ 2 ] ~ [ 8 ] 之中，有任一為 "W" 時，則 [ 1 ] = "W"</p><p>當 [ 2 ] ~ [ 8 ] 皆為 " " 時，則 [ 1 ] = " "</p> |
| SQLCA.SQLWARN \[ 2 ] | <p>當因資料過長，而被截掉時，則 [ 2 ] = "W"</p><p>反之則 [ 2 ] = " "</p>                                         |
| SQLCA.SQLWARN \[ 3 ] | <p>當 Aggregate Function 為 NULL 時，則 [ 3 ] = "W"</p><p>反之則 [ 3 ] = " "</p>                        |
| SQLCA.SQLWARN \[ 4 ] | <p>當查詢之欄位數量與 INTO 敘述欄位數量不相符時，<br>則 [ 4 ] = "W" ，反之則 [ 4 ] = " "</p>                             |
| SQLCA.SQLWARN \[ 5 ] | <p>當 FLOAT 資料型別轉成 INTEGER 資料型別時，</p><p>則 [ 5 ] = "W" ，反之則 [ 5 ] = " "</p>                       |
| SQLCA.SQLWARN \[ 6 ] | Informix-4GL 保留字，尚未使用                                                                           |
| SQLCA.SQLWARN \[ 7 ] | Informix-4GL 保留字，尚未使用                                                                           |
| SQLCA.SQLWARN \[ 8 ] | Informix-4GL 保留字，尚未使用                                                                           |

{% hint style="danger" %}
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/46000156-informix-4gl-%E7%B3%BB%E7%B5%B1%E5%85%A7%E5%AE%9A%E7%B8%BD%E9%AB%94%E8%AE%8A%E6%95%B8%E3%80%8A-sqlca-%E3%80%8B\(-%E5%85%AD-\)) 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
