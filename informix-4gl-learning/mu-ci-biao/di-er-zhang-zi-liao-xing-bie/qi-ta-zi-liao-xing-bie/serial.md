---
description: Informix-4GL 資料型別說明_SERIAL 資料型態
---

# SERIAL

#### 說明

| 語法   | SERIAL                                                                                       |
| ---- | -------------------------------------------------------------------------------------------- |
|      | SERIAL( n )                                                                                  |
| 資料長度 | 4 byte                                                                                       |
| 資料範圍 | 1 \~ 2147483647                                                                              |
| 說明   | <p>1.每一資料表只有一個 SERIAL ，設定後無法改變序號</p><p>2.若序號被刪除，則此刪除序號號碼將無法被使用</p><p>3.新增資料時，系統會自動累加新增號碼</p> |

#### 範例一

```objectivec
DEFINE employeeNum SERIAL
```

說明： employeeNum 起始值為 1 ，後續新增資料會以此累加 1

#### 範例二

```objectivec
DEFINE employeeNum SERIAL(1001)
```

說明： employeeNum 起始值為 1001 ，後續新增資料會以此累加 1

{% hint style="danger" %}
前往【 [城市芒果留言區](https://give0714.pixnet.net/blog/post/46469062-informix-4gl-%E5%85%B6%E4%BB%96%E8%B3%87%E6%96%99%E5%9E%8B%E5%88%A5%E3%80%8A-serial-data-%E3%80%8B) 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
