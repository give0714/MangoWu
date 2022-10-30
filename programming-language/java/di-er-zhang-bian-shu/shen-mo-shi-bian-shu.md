---
description: Java 變數說明
---

# 甚麼是變數 ?

## 何為變數 ?

* 變數（Variable）是用來存放暫時的資料，以便後續的處理。

## 變數的操作

{% code title="DeclareVar.java" lineNumbers="true" %}
```java
public class DeclareVar {
    public static void main(String[] argv) {
    
    // 宣告一個名稱為 i 的變數
        int i;
        // 宣告一個名稱為 j 的變數，並將 20 放入變數內
        int j= 30;
        // 將 20 放入 i 這個變數內
        i = 20;
        System.out.println("i = " + i);
        System.out.println("j = " + j);
        
    }
}
```
{% endcode %}

{% code title="執行結果" %}
```
i = 20
j = 30
```
{% endcode %}

* "="\
  稱為指定運算符（Assignment Operator）。\
  功用為將資料放到變數中。
* "+"\
  稱為連接運算符（Concantenation Operator）。\
  功用為將兩段文字連接起來。
* 可在宣告變數的同時，就設定該變數的初值。

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
