---
description: Informix-4GL 狀態變數使用說明
---

# status 狀態變數

* status 為 Informix-4GL 定義之系統變數
* 執行系統時，用於檢測有無發生 ERROR 錯誤狀態，並告警的系統變數
* 無法檢測不屬於 ERROR 錯誤狀態
* 無需宣告 status 狀態變數
* 可依現況做調整

| 狀態變數的型態  | 說明                                                                   |
| -------- | -------------------------------------------------------------------- |
| 0        | 當成功執行敘述時                                                             |
| 負值       | 當執行敘述發生錯誤時                                                           |
| 100      | 當 FOREACH 敘述或 SELECT 敘述無法找到符合條件的列值時                                  |
| NOTFOUND | <p>當 FOREACH 敘述或 SELECT 敘述無法找到符合條件的列值時<br>當 FETCH 敘述的游標移到最後一列之外時</p> |

{% hint style="danger" %}
【 [M@nGo 留言區](https://give0714.pixnet.net/blog/post/45997441-informix-4gl-%E7%8B%80%E6%85%8B%E8%AE%8A%E6%95%B8) 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
