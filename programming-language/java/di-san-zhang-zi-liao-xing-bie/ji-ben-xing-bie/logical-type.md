---
description: Java 基本型別 Primitive Data Types 種類
---

# Logical Type

## 種類

|    型別   |   長度   |      值域      |   初值  | 使用建議 |  備註 |
| :-----: | :----: | :----------: | :---: | :--: | :-: |
| boolean | 8 bits | true / false | false |   X  |     |

## 範例

{% code title="UsingBoolean.java" lineNumbers="true" %}
```java
public class UsingBoolean {
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

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
