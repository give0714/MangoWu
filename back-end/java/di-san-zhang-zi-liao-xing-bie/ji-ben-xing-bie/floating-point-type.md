---
description: Java 基本型別 Primitive Data Types 種類
---

# Floating Point Type

## 種類

<table><thead><tr><th width="131" align="center">型別</th><th width="112" align="center">長度</th><th width="256" align="center">值域</th><th align="center">初值</th><th align="center">備註</th></tr></thead><tbody><tr><td align="center">float</td><td align="center">32 bits</td><td align="center">-3.4E38 ~ -1.4E-45<br>1.4E-45 ~ 3.4E38</td><td align="center">0.0F</td><td align="center"></td></tr><tr><td align="center">double</td><td align="center">64 bits</td><td align="center">-1.8E308 ~ -4.9E-324<br>4.9E-324 ~ 1.8E308</td><td align="center">0.0D<br>0.0</td><td align="center">預設</td></tr></tbody></table>

## 範例 1

{% code title="FloatingValue.java" lineNumbers="true" %}
```java
public class FloatingValue {
	public static void main(String[] args) {
		
		float f1 = 0.01f;
		System.out.println("變數 f1 的內容為 " +f1);
		float f2 = 0.98f;
		System.out.println("變數 f2 的內容為 " +f2);
		float f3 = f1 + f2;
		System.out.println("f1 + f2 為 " +f3);

	}
}
```
{% endcode %}

{% code title="執行結果" %}
```
變數 f1 的內容為 0.01
變數 f2 的內容為 0.98
f1 + f2 為 0.99
```
{% endcode %}

## 範例 2

{% code title="DoubleValue.java" lineNumbers="true" %}
```java
public class DoubleValue {
	public static void main(String[] args) {
		
		double d1 = 3.4;
		System.out.println("變數 d1 的內容為 " +d1);
		double d2 = 3.0;
		System.out.println("變數 d2 的內容為 " +d2);
		double d3 = 0.1234;
		System.out.println("變數 d3 的內容為 " +d3);
		double d4 = 4;
		System.out.println("變數 d4 的內容為 " +d4);
		double d5 = .1234;
		System.out.println("變數 d5 的內容為 " +d5);
		double d6 = 2.0E-3;
		System.out.println("變數 d6 的內容為 " +d6);
		double d7 = 2.022_140_78E23;
		System.out.println("變數 d7 的內容為 " +d7);
		
	}
}
```
{% endcode %}

{% code title="執行結果" %}
```
變數 d1 的內容為 3.4
變數 d2 的內容為 3.0
變數 d3 的內容為 0.1234
變數 d4 的內容為 4.0
變數 d5 的內容為 0.1234
變數 d6 的內容為 0.002
變數 d7 的內容為 2.02214078E23
```
{% endcode %}

{% hint style="info" %}
說明：

* float 型別的數值最後必須加上 f 或 F，否則會被視為 double，而造成編譯錯誤。
* 會造成失真。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}

