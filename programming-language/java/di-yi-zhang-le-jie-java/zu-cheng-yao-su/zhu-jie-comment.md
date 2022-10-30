---
description: Java 程式的基本要素
---

# 註解 Comment

{% code title="FourthJava.java" lineNumbers="true" %}
```java
// 所要撰寫的第一個有註解的程式
public class FourthJava {
    public static void main(String[] argv) {
    // 前兩行都是固定的程式骨架

        // 在 main() 區塊中要執行的程式
        System.out.println
        ("自己編寫的第四支 Java 程式");
        System.out.println
        ("程式裡有註解!!");

    // 以下也是固定的程式骨架
    } // main() 區塊的結束括號
} // FourthJava 區塊的結束括號
```
{% endcode %}

{% code title="執行結果" %}
```
自己編寫的第四支 Java 程式
程式裡有註解!!
```
{% endcode %}

* 每個程式區塊是由一或多個敘述（Statement）所構成。
* 簡單的敘述以分號【;】結尾，有些複雜的敘述會以一個區塊作為結尾。
* 同一個敘述可以分成多行撰寫，和寫成一行的效果是一樣的。\
  <mark style="color:blue;background-color:blue;">※ 讀者建議寫還是要成一行，以增加辨識度及閱讀性。</mark>
* 敘述可由一或多個字符（Token）所組成。
* 字符與字符之間可以加上適當數量的空白符號（Whitespace），以方便辨識。
* 空白字元、換行字元及定位字元，都可以作為空白符號。
* "("、")"、"{"、"}"、"\["、"]"、";"、","、"."，稱為分隔符號（Separator / punctuator）。

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
