---
description: Java 基本型別 Primitive Data Types 種類
---

# Textual Type

## 種類

|  型別  |    長度   |                   值域                   |    初值    | 使用建議 |  備註 |
| :--: | :-----: | :------------------------------------: | :------: | :--: | :-: |
| char | 16 bits | <p>'\u0000' ~ 'uffff'<br>0 ~ 65535</p> | '\u0000' |      |     |

## 範例

{% code title="TextualValue.java" lineNumbers="true" %}
```java
public class TextualValue {
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
變數 c1 的內容為 b
變數 c2 的內容為 中
變數 c3 的內容為 b
char 型別的 < u5b57 > 為 字
```
{% endcode %}

{% hint style="info" %}
說明：

* char 型別的內碼為 unicode 字源字碼。
{% endhint %}

## 跳脫序列 Escape Sequence

| 跳脫序列 |   字碼   |      字元     |  備考 |
| :--: | :----: | :---------: | :-: |
|  \b  | \u0008 | 按下 Enter 退格 |     |
|  \t  | \u0009 |  按下 Tab 跳八格 |     |
|  \n  | \u000a |      換行     |     |
|  \f  | \u000c |      換頁     |     |
|  \r  | \u000d |      返回     |     |
|  \\" | \u0022 |     雙引號     |     |
|  \\' | \u0027 |     單引號     |     |
| \\\\ | \u005c |     反斜線     |     |

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}

