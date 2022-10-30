---
description: Java 變數說明
---

# 變數的名稱

## 命名規則

1. 駝峰式命名方式\
   變數如由一個以上的英文字組成，則英文字之間沒有空格。\
   第一個英文字由小寫組成，之後的英文字則為大寫組成。
2. 須以英文字母為開頭，或以 "\_" 或 "$" 這兩個字元開頭。\
   <mark style="color:blue;background-color:blue;">※ Java 編譯器在編譯程式過程中，可能會需要建立開頭以 "$" 的額外變數，</mark>\
   &#x20;  <mark style="color:blue;background-color:blue;">可能會造成閱讀程式的人產生混淆，所以建議不要這樣使用。</mark>
3. 除第一個字元外，還可使用 0 \~ 9 的數字。
4. 沒有命名長度限制。
5. 不能使用保留字（Keyward）來命名。
6. 不能使用字面常數（Literal）來命名。
7. 如果命名兩個字母均相同的變數，但大小寫不同時，會被視為不同的變數。
8. 可使用許多標準萬國碼（Unicode）的字原來命名。
9. 可使用中文來命名變數，但還是建議不要這樣使用。

## 識別字命名慣用型式

* <mark style="color:red;">class</mark> & <mark style="color:red;">interface</mark> 類別和介面\
  CustomerName
* <mark style="color:red;">methon</mark> & <mark style="color:red;">variable</mark> 函數和變數\
  customerName
* <mark style="color:red;">constant</mark> 常數變數\
  CUSTOMER\_COUNT

{% hint style="warning" %}
建置中...
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
