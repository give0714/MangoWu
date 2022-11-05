---
description: Java 程式的基本要素
---

# 註解 Comment

## 單行註解

{% code title="FourthJava.java" lineNumbers="true" %}
```java
// 所要撰寫的第一個有註解的程式
public class FourthJava {
    @Annotation
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

* // ...\
  字符往後一直到該行文字結束之前的內容，都是註解，稱為單行註解（End-Of-Line Comment）。

## 多行註解

{% code title="FifthJava.java" lineNumbers="true" %}
```java
/* 所要撰寫的有多行註解的程式
   版本：V 1.0
 */
public class FifthJava {
    public static void main(String[] argv) {
    /* 前兩行都是固定的程式骨架 */

        // 在 main() 區塊中要執行的程式
        System.out.println
        ("自己編寫的第五支 Java 程式");
        System.out.println
        ("程式裡有註解!!");

    /* 以下也是固定的程式骨架 */
    } // main() 區塊的結束括號
} // FifthJava 區塊的結束括號
```
{% endcode %}

{% code title="執行結果" %}
```
自己編寫的第五支 Java 程式
程式裡有註解!!
```
{% endcode %}

* /\* ...\
  &#x20;   ...\
  &#x20;   ...\
  \*/\
  這種可以跨越多行的註解方式，稱為傳統式註解（Traditional Comment）\
  &#x20;                                               或區塊式註解（Block Comment），\
  以成對的 /\* 及 \*/ 來包含所要加入的註解說明。

## 文件註解

{% code title="SixthJava.java" lineNumbers="true" %}
```java
/** 第一行註解文字
    第二行註解文字
    ... */
public class SixthJava {
    public static void main(String[] argv) {
    /* 前兩行都是固定的程式骨架 */

        // 在 main() 區塊中要執行的程式
        System.out.println
        ("自己編寫的第六支 Java 程式");
        System.out.println
        ("程式裡有註解!!");

    /* 以下也是固定的程式骨架 */
    } // main() 區塊的結束括號
} // FifthJava 區塊的結束括號
```
{% endcode %}

{% code title="執行結果" %}
```
自己編寫的第六支 Java 程式
程式裡有註解!!
```
{% endcode %}

## Annotation 註解【JDK 5.0 以後才有的語法】

* @Override
* @Deprecated
* @SuppressWarnings



{% hint style="info" %}
說明：

註解是一項非必要，但建議一定要使用的工具。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
