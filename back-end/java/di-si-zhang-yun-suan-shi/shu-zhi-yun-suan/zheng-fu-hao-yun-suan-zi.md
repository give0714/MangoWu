---
description: Java 運算式說明章節
---

# 正、負號運算子

### 種類

* \+ var 正號運算子
* \- var 負號運算子

{% code title="Minus.java" lineNumbers="true" %}
```java
public class Minus {

	public static void main(String[] args) {
		
		int i = 7;
		int j = -i;
		System.out.println("i = " + i );
		System.out.println("j = " + j );
		
		int k = i - j;
		System.out.println("k = i - j =>> " + k );

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
i = 7
j = -7
k = i - j =>> 14
```
{% endcode %}

{% hint style="info" %}
備註：

* 除可當作加法與減法的算符外，也可以當作為單一運算元的正、負號算符。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
