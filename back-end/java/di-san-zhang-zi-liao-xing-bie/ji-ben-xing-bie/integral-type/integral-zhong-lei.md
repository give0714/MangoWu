---
description: Java 基本型別 Primitive Data Types 種類
---

# Integral 種類

## 種類

<table><thead><tr><th width="117" align="center">型別</th><th width="103" align="center">長度</th><th width="262" align="center">值域</th><th width="94" align="center">初值</th><th width="98" align="center">使用建議</th><th width="73" align="center">備註</th></tr></thead><tbody><tr><td align="center">byte</td><td align="center">8 bits</td><td align="center">-2 的  7次方 ~ 2 的  7次方 - 1<br><mark style="color:blue;">-128 ~ 127</mark></td><td align="center">0</td><td align="center">X</td><td align="center"></td></tr><tr><td align="center">short</td><td align="center">16 bits</td><td align="center">-2 的 15次方 ~ 2 的 15次方 - 1<br><mark style="color:blue;">-32768 ~ 32767</mark></td><td align="center">0</td><td align="center">X</td><td align="center"></td></tr><tr><td align="center">int</td><td align="center">32 bits</td><td align="center">-2 的 31次方 ~ 2 的 31次方 - 1<br><mark style="color:blue;">-2147483648 ~ 2147483647</mark></td><td align="center">0</td><td align="center"></td><td align="center">預設</td></tr><tr><td align="center">long</td><td align="center">64 bits</td><td align="center">-2 的 63次方 ~ 2 的 63次方 - 1<br><mark style="color:blue;">-9223372036854775808 ~ 9223372036854775807</mark></td><td align="center">0L / 0l</td><td align="center"></td><td align="center"></td></tr></tbody></table>

## 範例

{% code title="UsingIntegral.java" lineNumbers="true" %}
```java
public class UsingIntegral {
       public static void main(String[] args) {

              byte b = 127;
              System.out.println("byte 變數 b 的值：" + b);
              short s = 32767;
              System.out.println("short 變數 s 的值：" + s);
              int i = 2147483647;
              System.out.println("int 變數 i 的值：" + i);
              long l = 9223372036854775807L;
              System.out.println("long 變數 l 的值：" + l);              

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

{% hint style="info" %}
說明：

* 不會造成失真。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
