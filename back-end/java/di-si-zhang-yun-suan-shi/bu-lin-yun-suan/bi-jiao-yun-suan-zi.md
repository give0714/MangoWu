---
description: Java 運算式說明章節
---

# 比較運算子

## 比較運算子 Comparison Operator

### 種類

* num1 == num2   比較左邊的運算元是否等於右邊的運算元
* num1 != num2    比較左邊的運算元是否不等於右邊的運算元
* num1 > num2     比較左邊的運算元是否大於右邊的運算元
* num1 >= num2   比較左邊的運算元是否大於等於右邊的運算元
* num1 < num2     比較左邊的運算元是否小於右邊的運算元
* num1 <= num2   比較左邊的運算元是否小於等於右邊的運算元

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

## 遞減運算子 Decrement Operator

### 種類

* var-- 後置型 Postfix
* \--var 前置型 Prefix

{% code title="Decrement.java" lineNumbers="true" %}
```java
public class Decrement {

	public static void main(String[] args) {
		
		int b = 10;
		System.out.println("b = " + b);
		System.out.println("前置型遞減運算元為 " + (--b));
		System.out.println("b = " + b);
		System.out.println("後置型遞減運算元為 " + (b--));
		System.out.println("b = " + b);

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
b = 10
前置型遞減運算元為 9
b = 9
後置型遞減運算元為 9
b = 8
```
{% endcode %}

{% hint style="info" %}
備註：

* 前置型：\
  當遞增或遞減運算子放置於變數前面，運算結果會是變數遞增後或遞減後的數值。
* 後置型：\
  當遞增或遞減運算子放置於變數後面，運算結果會是變數遞增前或遞減前的原始數值。
* 只能用於變數上。
* 可用在整數數值型別，也可以用在浮點數數值型別。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
