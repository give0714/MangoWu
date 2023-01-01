---
description: Java 運算式說明章節
---

# 比較運算子

## 比較運算子 Comparison Operator

### 種類

* num1 == num2   比較左邊的運算元是否等於右邊的運算元
* num1 !=  num2   比較左邊的運算元是否不等於右邊的運算元
* num1 >   num2   比較左邊的運算元是否大於右邊的運算元
* num1 >= num2   比較左邊的運算元是否大於等於右邊的運算元
* num1 <   num2   比較左邊的運算元是否小於右邊的運算元
* num1 <= num2   比較左邊的運算元是否小於等於右邊的運算元

{% code title="Comparison.java" lineNumbers="true" %}
```java
public class Comparison {

	public static void main(String[] args) {
		
		int i = 4, j = 5;
		System.out.println("當 i 為 " + i + " , j 為 " + j );
		System.out.println("i == j ==>> " + ( i == j ) );
		System.out.println("i != j ==>> " + ( i != j ) );
		System.out.println("i >  j ==>> " + ( i >  j ) );
		System.out.println("i >= j ==>> " + ( i >= j ) );
		System.out.println("i <  j ==>> " + ( i <  j ) );
		System.out.println("i <= j ==>> " + ( i <= j ) );

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
當 i 為 4 , j 為 5
i == j ==>> false
i != j ==>> true
i >  j ==>> false
i >= j ==>> false
i <  j ==>> true
i <= j ==>> true
```
{% endcode %}

{% hint style="info" %}
備註：

* \== 與 != 可用於數值的比較，也可用於布林值的比較。
* 因浮點數是以二進位來表示小數點，有時無法精準表示十進位的小數值，會有產生誤差值，所以要避免做浮點數的比較運算。
* 比較運算子的運算結果是一個布林值，代表所比較的關係是否成立。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
