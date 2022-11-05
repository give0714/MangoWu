---
description: Java 基本型別 Primitive Data Types 種類
---

# Integral 進制設定

## 種類

|  進位方式 |        說明        |        例如       |  備註 |
| :---: | :--------------: | :-------------: | :-: |
|  2 進位 | 為 0b 或 0B 開頭的數值。 |  0b1010、0B1010  |     |
|  8 進位 |    為 0 開頭的數值。    |       012       |     |
| 10 進位 |    為非 0 開頭的數值。   |        10       |     |
| 16 進位 | 為 0x 或 0X 開頭的數字。 | 0xa、0xA、0Xa、0XA |     |

## 範例

{% code title="IntegerValue.java" lineNumbers="true" %}
```java
public class IntegerValue {
  public static void main(String[] args) {
		    
int a = 10;
	System.out.println("a 為：" + a);
	System.out.print("a的二進位為：0b" + Integer.toBinaryString(a));
	System.out.println(" 或 0B" + Integer.toBinaryString(a));
	System.out.println("a的八進位為：0" + Integer.toOctalString(a));
	System.out.print("a的十六進位為：0x" + Integer.toHexString(a));
	System.out.print(" 或 0X" + Integer.toHexString(a).toUpperCase());
	System.out.print(" 或 0X" + Integer.toHexString(a));
	System.out.println(" 或 0X" + Integer.toHexString(a).toUpperCase());
	
  }
}
```
{% endcode %}

{% code title="執行結果" %}
```
byte 變數 b 的值：127
short 變數 s 的值：32767
int 變數 i 的值：2147483647
long 變數 l 的值：9223372036854775807
```
{% endcode %}

{% hint style="warning" %}
建置中...
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
