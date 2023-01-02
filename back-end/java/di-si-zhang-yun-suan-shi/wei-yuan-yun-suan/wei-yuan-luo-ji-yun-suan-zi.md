---
description: Java 運算式說明章節
---

# 位元邏輯運算子

## 位元邏輯運算子 Bitwise Logical Operator

### 種類

* int1  |  int2
* int1 &  int2
* int1  ^  int2

{% code title="BitwiseLogical.java" lineNumbers="true" %}
```java
public class BitwiseLogical {

	public static void main(String[] args) {
		
		byte b1 = 2;
		byte b2 = -2;
		System.out.println("b1 =  " + b1 + " , 二進制為 00000010" );
		System.out.println("b2 = " + b2 + " , 二進制為 11111110" );
		System.out.println("b1 | b2 = " + ( b1 | b2 ) );
		System.out.println("      00000010");
		System.out.println("    | 11111110");
		System.out.println("=>>   11111110");
		System.out.println("b1 & b2 = " + ( b1 & b2 ) );
		System.out.println("      00000010");
		System.out.println("    & 11111110");
		System.out.println("=>>   00000010");
		System.out.println("b1 ^ b2 = " + ( b1 ^ b2 ) );
		System.out.println("      00000010");
		System.out.println("    ^ 11111110");
		System.out.println("=>>   11111100");


	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
b1 =  2 , 二進制為 00000010
b2 = -2 , 二進制為 11111110

b1 | b2 = -2
      00000010
    | 11111110
=>>   11111110

b1 & b2 = 2
      00000010
    & 11111110
=>>   00000010

b1 ^ b2 = -4
      00000010
    ^ 11111110
=>>   11111100
```
{% endcode %}

{% hint style="info" %}
備註：

* 位元邏輯運算子一律會將兩邊運算元的值都求出來，兩邊的運算元必須是布林型別，或是整數型別。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
