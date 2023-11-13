---
description: Java 基本型別 Primitive Data Types 種類
---

# Integral 進制設定

## 種類

<table><thead><tr><th width="117" align="center">進位方式</th><th width="307" align="center">說明</th><th width="211" align="center">例如</th><th width="113" align="center">備註</th></tr></thead><tbody><tr><td align="center">2 進位</td><td align="center">為 0b 或 0B 開頭的數值。</td><td align="center">0b1010、0B1010</td><td align="center"></td></tr><tr><td align="center">8 進位</td><td align="center">為 0 開頭的數值。</td><td align="center">012</td><td align="center"></td></tr><tr><td align="center">10 進位</td><td align="center">為非 0 開頭的數值。</td><td align="center">10</td><td align="center"></td></tr><tr><td align="center">16 進位</td><td align="center">為 0x 或 0X 開頭的數字。</td><td align="center">0xa、0xA、0Xa、0XA</td><td align="center"></td></tr></tbody></table>

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
a 為：10
a 的二進位為：0b1010 或 0B1010
a 的八進位為：012
a 的十六進位為：0xa 或 0XA 或 0Xa 或 0XA
```
{% endcode %}

{% hint style="info" %}
說明：

* 輸出數值時，預設為十進位表示。
* 預設為正數。
* 預設為 int 型別，如果要表示為 long 型別，就必須在數值後面加上 L 或 l。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
