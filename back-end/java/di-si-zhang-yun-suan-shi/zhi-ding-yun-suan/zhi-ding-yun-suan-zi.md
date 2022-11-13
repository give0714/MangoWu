---
description: Java 運算式說明章節
---

# 指定運算子

## 指定運算子 Assignment Operator

<img src="../../../../.gitbook/assets/file.drawing (1).svg" alt="" class="gitbook-drawing">

### 指定變數的用法

{% code title="Assignment.java" lineNumbers="true" %}
```java
public class Assignment {

	public static void main(String[] args) {
		
		int i, j = 1;
		i = 0;
		System.out.print("放入數值 ");
		System.out.println("i = " + i);
		i = j;
		System.out.print("放入變數 ");
		System.out.println("i = " + i);
		System.out.println("      j = " + j);
		i = 4 * 5;
		System.out.print("放入運算式 ");
		System.out.println("i = " + i);
		boolean b;
		b = true;
		System.out.print("放入字面常數 ");
		System.out.println("b = " + b);

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
放入數值 i = 0
放入變數 i = 1
        j = 1
放入運算式 i = 20
放入字面常數 b = true
```
{% endcode %}

### 同時指定給多個變數

{% code title="AssignmentToAll.java" lineNumbers="true" %}
```java
public class AssignmentToAll {

	public static void main(String[] args) {
		
		int i, j, k, l;
		i = j = k = l = 2;
		System.out.println("i = " + i);
		System.out.println("j = " + j);
		System.out.println("k = " + k);
		System.out.println("l = " + l);

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
i = 2
j = 2
k = 2
l = 2
```
{% endcode %}

{% hint style="info" %}
備註：

* 指定運算子用來設定變數的內容。
* "<mark style="color:red;">**=**</mark>" 並不是數學上等於的意思，而是 "<mark style="color:blue;">**指定**</mark>" 的意思
* 需要 2 個運算元。
* 左邊的運算元必須是一個變數，右邊的運算元可以是變數、字面常數、運算式。
* 右邊運算元的位階不可高於左邊運算元的位階。
  * double > float > long > int > short > byte
* 運算子的作用：
  * 如果右邊的運算元是一個運算式，就是把右邊運算式的結果放入左邊的變數內。
  * 如果右邊的運算元是一個變數，就是把右邊變數值放入左邊的變數內。
  * 如果右邊的運算元是一個字面常數，就直接將右邊常數值放入左邊的變數內。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
