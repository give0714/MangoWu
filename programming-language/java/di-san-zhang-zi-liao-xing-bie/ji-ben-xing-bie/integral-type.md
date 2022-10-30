---
description: Java 基本型別 Primitive Data Types 種類
---

# Integral Type

## 簡介

|   型別  |    長度   |             值域            |   初值   |  備註 |
| :---: | :-----: | :-----------------------: | :----: | :-: |
|  byte |  8 bits | -2 的  7次方 \~ 2 的  7次方 - 1 |    0   |     |
| short | 16 bits | -2 的 15次方 \~ 2 的 15次方 - 1 |    0   |     |
|  int  | 32 bits | -2 的 31次方 \~ 2 的 31次方 - 1 |    0   |  預設 |
|  long | 64 bits | -2 的 63次方 \~ 2 的 63次方 - 1 | 0L / 0 |     |

## 範例

{% code title="UsingBoolean.java" lineNumbers="true" %}
```java
public class UsingBoolean{
       public static void main(String[] args) {

              boolean test = false;
              System.out.println("布林變數 test 的值：" + test);
              test = true;
              System.out.println("布林變數 test 的值：" + test);

       }
}
```
{% endcode %}

{% code title="執行結果" %}
```
布林變數 test 的值：false
布林變數 test 的值：true
```
{% endcode %}

{% hint style="warning" %}
建置中...
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
