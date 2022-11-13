---
description: Java 運算式說明章節
---

# 二元運算子

## 二元運算子 Binary Operator

{% code title="BinaryOperator.java" lineNumbers="true" %}
```java
public class BinaryOperator{

       public static void main(String[] args) {

              int i = 2 + 1;
              System.out.println("二元運算子 i 的值：" + i);
              int j = i +1;
              System.out.println("二元運算子 j 的值：" + j);
              int k = i + j;
              System.out.println("二元運算子 k 的值：" + k);
              
       }
       
}
```
{% endcode %}

{% code title="執行結果" %}
```
二元運算子 i 的值：3
二元運算子 j 的值：4
二元運算子 k 的值：7
```
{% endcode %}

{% hint style="info" %}
備註：

* 如果運算子需要二個運算元，就可稱為二元運算子（Binary Operator）。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
