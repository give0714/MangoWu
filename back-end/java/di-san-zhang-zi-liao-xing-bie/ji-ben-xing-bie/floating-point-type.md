---
description: Java 基本型別 Primitive Data Types 種類
---

# Floating Point Type

## 種類

|   型別   |    長度   |                         值域                        |         初值         |  備註 |
| :----: | :-----: | :-----------------------------------------------: | :----------------: | :-: |
|  float | 32 bits |   <p>-3.4E38 ~ -1.4E-45<br>1.4E-45 ~ 3.4E38</p>   |        0.0F        |     |
| double | 64 bits | <p>-1.8E308 ~ -4.9E-324<br>4.9E-324 ~ 1.8E308</p> | <p>0.0D<br>0.0</p> |     |

## 範例 1

{% code title="FloatingValue.java" lineNumbers="true" %}
```java
public class FloatingValue {
    public static void main(String[] args) {
		
        char c1 = 'b';
        System.out.println("變數 c1 的內容為 " + c1);
        char c2 = '中';
        System.out.println("變數 c2 的內容為 " + c2);
        char c3 = 98;
        System.out.println("變數 c3 的內容為 " + c3);
        char c4 = '\u5b57';
        System.out.println("char 型別的 < \u5b57 > 為 " + c4);
        
    }
}
```
{% endcode %}

{% code title="執行結果" %}
```
```
{% endcode %}

## 範例 2

{% code title="DoubleValue.java" lineNumbers="true" %}
```java
public class DoubleValue {
    public static void main(String[] args) {
		
        char c1 = 'b';
        System.out.println("變數 c1 的內容為 " + c1);
        char c2 = '中';
        System.out.println("變數 c2 的內容為 " + c2);
        char c3 = 98;
        System.out.println("變數 c3 的內容為 " + c3);
        char c4 = '\u5b57';
        System.out.println("char 型別的 < \u5b57 > 為 " + c4);
        
    }
}
```
{% endcode %}

{% code title="執行結果" %}
```
```
{% endcode %}

{% hint style="warning" %}

{% endhint %}

{% hint style="warning" %}
建置中...
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}

