---
description: Java 運算式說明章節
---

# 遞增、遞減運算子

## 遞增運算子 Increment Operator

### 種類

* var++ 後置型
* \++var 前置型

{% code title="Increment.java" lineNumbers="true" %}
```java
public class Increment {

	public static void main(String[] args) {
		
		int i = 1;
		System.out.println("i      = " + i);
		i = i + 1;
		System.out.println("i + 1  = " + i);
		i = i - 1;
		System.out.println("i - 1  = " + i);
		i = i * 10;
		System.out.println("i * 10 = " + i);
		i = i / 2;
		System.out.println("i / 5  = " + i);
		i = i % 2;
		System.out.println("i % 3  = " + i);

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
i      = 1
i + 1  = 2
i - 1  = 1
i * 10 = 10
i / 5  = 5
i % 3  = 1
```
{% endcode %}

## 遞減運算子 Decrement Operator

### 種類

* var--
* \--var

{% code title="Decrement.java" lineNumbers="true" %}
```java
public class Decrement {

	public static void main(String[] args) {
		
		int i = 1;
		System.out.println("i      = " + i);
		i = i + 1;
		System.out.println("i + 1  = " + i);
		i = i - 1;
		System.out.println("i - 1  = " + i);
		i = i * 10;
		System.out.println("i * 10 = " + i);
		i = i / 2;
		System.out.println("i / 5  = " + i);
		i = i % 2;
		System.out.println("i % 3  = " + i);

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
i      = 1
i + 1  = 2
i - 1  = 1
i * 10 = 10
i / 5  = 5
i % 3  = 1
```
{% endcode %}

{% hint style="warning" %}
建置中
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
