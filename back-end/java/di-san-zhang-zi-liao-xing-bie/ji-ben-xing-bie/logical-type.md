---
description: Java 基本型別 Primitive Data Types 種類
---

# Logical Type

## 種類

<table><thead><tr><th width="116" align="center">型別</th><th width="103" align="center">長度</th><th width="262" align="center">值域</th><th width="79" align="center">初值</th><th align="center">使用建議</th><th width="89" align="center">備註</th></tr></thead><tbody><tr><td align="center">boolean</td><td align="center"></td><td align="center">true / false</td><td align="center">false</td><td align="center">X</td><td align="center"></td></tr></tbody></table>

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
