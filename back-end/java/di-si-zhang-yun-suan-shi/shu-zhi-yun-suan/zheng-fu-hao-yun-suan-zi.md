---
description: Java 運算式說明章節
---

# 正、負號運算子

### 種類

* \+ var 正號運算子
* \- var 負號運算子

{% code title="Increment.java" lineNumbers="true" %}
```java
public class Increment {

	public static void main(String[] args) {
		
		int a = 10;
		System.out.println("a = " + a);
		System.out.println("前置型遞增運算元為 " + (++a));
		System.out.println("a = " + a);		
		System.out.println("後置型遞增運算元為 " + (a++));
		System.out.println("a = " + a);

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
a = 10
前置型遞增運算元為 11
a = 11
後置型遞增運算元為 11
a = 12
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
