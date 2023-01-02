---
description: Java 運算式說明章節
---

# 邏輯運算子

## 邏輯運算子 Logical Operator

### 種類

* opr1  ^  opr2
* opr1  &  opr2
* opr1   |  opr2
* opr1 && opr2
* opr1  ||  opr2

#### 範例 1

{% code title="Logical.java" lineNumbers="true" %}
```java
public class Logical {

	public static void main(String[] args) {
		
		boolean i = true, j = false;
		System.out.println("當 i 為 " + i + ", j 為 " + j );
		System.out.println("i  & j 為 " + ( i  & j ) );
		System.out.println("i && j 為 " + ( i && j ) );
		System.out.println("i  | j 為 " + ( i  | j ) );
		System.out.println("i || j 為 " + ( i || j ) );
		System.out.println("i  ^ j 為 " + ( i  ^ j ) );

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
當 i 為 true, j 為 false
i  & j 為 false
i && j 為 false
i  | j 為 true
i || j 為 true
i  ^ j 為 true
```
{% endcode %}

#### 範例 2

{% code title="ShortCircuit.java" lineNumbers="true" %}
```java
public class ShortCircuit {

	public static void main(String[] args) {
		
		int i = 3, j = 4;
		System.out.println("當 i 為 " + i + " , j 為 " + j );
		System.out.println("使用 | 的運算結果為");
		System.out.println("i++ == j =>> " + ( true | ( i++ == j ) ) );
		System.out.println("現在 i 為 " + i + " , j 為 " + j );
		i = 3;
		j = 4;
		System.out.println("當 i 為 " + i + " , j 為 " + j );
		System.out.println("i++ == j =>> " + ( true || ( i++ == j ) ) );
		System.out.println("使用 || 的運算結果為");
		System.out.println("現在 i 為 " + i + " , j 為 " + j );

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
當 i 為 3 , j 為 4
使用 | 的運算結果為
i++ == j =>> true
現在 i 為 4 , j 為 4

當 i 為 3 , j 為 4
i++ == j =>> true
使用 || 的運算結果為
現在 i 為 3 , j 為 4
```
{% endcode %}

{% hint style="info" %}
備註：

* 邏輯運算子為布林資料的比較運算，需要兩個布林型別的運算元。
* 各個運算子的意義
  1. & 與 &&\
     AND （且）- 當兩個運算元皆為 true 時，結果才為 true，否則為 false。
  2. &#x20;\| 與  ||\
     OR（或）- 只要兩個運算元的其中一個為 true 時，結果就為 true，否則為 false。
  3. &#x20;^\
     互斥（XOR）- 當兩個運算元皆為不同時，結果才為 true，否則為 false。
* && 與  ||  會在左邊運算元就可以決定運算結果的情況下，忽略右邊的運算元，所以又被稱為條件運算子（Conditional Operator）。\
  只靠左邊即可推算運算結果，而忽略右邊的方式，稱為短路模式（Short Circuit）。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}

