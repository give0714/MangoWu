---
description: Java 運算式說明章節
---

# 算術運算子

## 算術運算子 Arithmetic Operator

## 種類

1. \+   加
2. \-   減
3. \*   乘
4. /    除
5. %  求餘數

{% code title="Arithmetic.java" lineNumbers="true" %}
```java
public class Arithmetic {

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

{% hint style="info" %}
備註：

* 若兩個運算元的位階不相等，運算後的位階會與運算元位階高者相同。
* 若兩個運算元為基本型別，至少會轉換成 int 型別。
* 若兩個運算元皆為數字，則執行該運算。
* 在加法運算子的運算式中，若有一個運算元為 String，則執行串接運算。
* 運算的優先順序：
  * &#x20;\*、/、% -> +、-
  * 小括號內的優先
  * 當優先順序相同時，則由左至右來運算。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
