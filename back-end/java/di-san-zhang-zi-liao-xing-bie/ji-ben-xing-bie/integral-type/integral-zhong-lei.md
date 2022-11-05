---
description: Java 基本型別 Primitive Data Types 種類
---

# Integral 種類

## 種類

|   型別  |    長度   |                                                       值域                                                       |    初值   | 使用建議 |  備註 |
| :---: | :-----: | :------------------------------------------------------------------------------------------------------------: | :-----: | :--: | :-: |
|  byte |  8 bits |                 <p>-2 的  7次方 ~ 2 的  7次方 - 1<br><mark style="color:blue;">-128 ~ 127</mark></p>                 |    0    |   X  |     |
| short | 16 bits |               <p>-2 的 15次方 ~ 2 的 15次方 - 1<br><mark style="color:blue;">-32768 ~ 32767</mark></p>               |    0    |   X  |     |
|  int  | 32 bits |          <p>-2 的 31次方 ~ 2 的 31次方 - 1<br><mark style="color:blue;">-2147483648 ~ 2147483647</mark></p>          |    0    |      |  預設 |
|  long | 64 bits | <p>-2 的 63次方 ~ 2 的 63次方 - 1<br><mark style="color:blue;">-9223372036854775808 ~ 9223372036854775807</mark></p> | 0L / 0l |      |     |

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

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
