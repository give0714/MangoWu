---
description: Java 運算式說明章節
---

# 複合指定運算子

## 複合指定運算子 Compound Assignment Operator

## 種類

1. \+=\
   範例說明：\
   &#x20;                i = i + 1;   =>   i += 1;
2. \-=\
   範例說明：\
   &#x20;                i = i - 1;   =>   i -= 1;
3. \*=\
   範例說明：\
   &#x20;                i = i \* 1;   =>   i \*= 1;
4. /=\
   範例說明：\
   &#x20;                i = i / 1;   =>   i /= 1;
5. %=\
   範例說明：\
   &#x20;                i = i % 1;   =>   i %= 1;

{% code title="CompoundAssignment.java" lineNumbers="true" %}
```java
public class CompoundAssignment {

	public static void main(String[] args) {
		
		int i = 5;
		System.out.println("i = " + i);
		System.out.println("i += 1 為 " + ( i += 1 ));
		System.out.println("i -= 1 為 " + ( i -= 1 ));
		System.out.println("i *= 5 為 " + ( i *= 5 ));
		System.out.println("i /= 5 為 " + ( i /= 5 ));
		System.out.println("i %= 3 為 " + ( i %= 3 ));

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
i  = 5
i += 1 為 6
i -= 1 為 5
i *= 5 為 25
i /= 5 為 5
i %= 3 為 2
```
{% endcode %}

{% hint style="info" %}
備註：

* 複合指定運算子會將左邊運算元的值取出，和右邊運算元運算之後，強制將運算結果轉回左邊運算元的型別，然後再放回左邊運算元內，故不需要自己撰寫轉換型別的動作。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
