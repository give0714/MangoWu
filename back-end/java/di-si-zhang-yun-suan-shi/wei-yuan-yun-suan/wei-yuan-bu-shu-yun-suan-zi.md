---
description: Java 運算式說明章節
---

# 位元補數運算子

## 位元補數運算子 Bitwise Complement Operator

### 種類

* \~var

{% code title="BitwiseComplement.java" lineNumbers="true" %}
```java
public class BitwiseComplement {

	public static void main(String[] args) {
		
		byte b1 = 127;
		System.out.println(" b1 =  " + b1 + " , 二進制為 01111111" );
		System.out.println("~b1 = " + (~b1) + " , 二進制為 10000000" );
		byte b2 = -1;
		System.out.println(" b2 =   " + b2 + " , 二進制為 11111111" );
		System.out.println("~b2 =    " + (~b2) + " , 二進制為 00000000" );

	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
 b1 =  127 , 二進制為 01111111
~b1 = -128 , 二進制為 10000000
 b2 =   -1 , 二進制為 11111111
~b2 =    0 , 二進制為 00000000
```
{% endcode %}

{% hint style="info" %}
備註：

* 位元補數運算子只需一個整數型別的運算元，運算結果就為取運算元的二進位補數。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
