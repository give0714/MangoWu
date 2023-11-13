---
description: Java 基本型別 Primitive Data Types 種類
---

# Textual Type

## 種類

<table><thead><tr><th width="93" align="center">型別</th><th width="89" align="center">長度</th><th width="273" align="center">值域</th><th width="102" align="center">初值</th><th width="98" align="center">使用建議</th><th width="73" align="center">備註</th></tr></thead><tbody><tr><td align="center">char</td><td align="center">16 bits</td><td align="center">'\u0000' ~ 'uffff'<br>0 ~ 65535</td><td align="center">'\u0000'</td><td align="center"></td><td align="center"></td></tr></tbody></table>

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

<table><thead><tr><th width="118" align="center">跳脫序列</th><th width="114" align="center">字碼</th><th width="329" align="center">字元</th><th width="189" align="center">備考</th></tr></thead><tbody><tr><td align="center">\b</td><td align="center">\u0008</td><td align="center">按下 Enter 退格</td><td align="center"></td></tr><tr><td align="center">\t</td><td align="center">\u0009</td><td align="center">按下 Tab 跳八格</td><td align="center"></td></tr><tr><td align="center">\n</td><td align="center">\u000a</td><td align="center">換行</td><td align="center"></td></tr><tr><td align="center">\f</td><td align="center">\u000c</td><td align="center">換頁</td><td align="center"></td></tr><tr><td align="center">\r</td><td align="center">\u000d</td><td align="center">返回</td><td align="center"></td></tr><tr><td align="center">\"</td><td align="center">\u0022</td><td align="center">雙引號</td><td align="center"></td></tr><tr><td align="center">\'</td><td align="center">\u0027</td><td align="center">單引號</td><td align="center"></td></tr><tr><td align="center">\\</td><td align="center">\u005c</td><td align="center">反斜線</td><td align="center"></td></tr></tbody></table>

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}

