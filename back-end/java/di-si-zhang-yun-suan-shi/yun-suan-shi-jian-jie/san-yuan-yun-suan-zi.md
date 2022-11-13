---
description: Java 運算式說明章節
---

# 三元運算子

## 三元運算子 Ternary Operator

{% code title="BinaryOperator.java" lineNumbers="true" %}
```java
public class BinaryOperator{

       public static void main(String[] args) {
		
		boolean b1 = true;
		String str1 = ( b1 ? "true" : "false");
		System.out.println( "b1 為" + str1);
		boolean b2 = !b1;
		String str2 = ( b2 ? "true" : "false");
		System.out.println( "b2 為" + str2);

	}
       
}
```
{% endcode %}

{% code title="執行結果" %}
```
b1 為true
b2 為false
```
{% endcode %}

{% hint style="info" %}
備註：

* 三元運算子（Ternary Operator）又稱為條件運算子（Conditional Operator）。
* 由 3 個運算元所組成，分別以 ? 與 : 區隔開來。&#x20;
* 第一個運算元必須為 boolean。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
