---
description: Java 基本型別 Primitive Data Types 種類
---

# Integral 進制設定

## 種類

| 進位方式 |  說明 | 使用建議 |  備註 |
| :--: | :-: | :--: | :-: |
|  2   |  0  |      |     |
|  8   |     |      |     |
|  10  |     |      |     |
|  16  |     |      |     |

## 範例

<pre class="language-java" data-title="UsingIntegral.java" data-line-numbers><code class="lang-java"><strong>public class UsingIntegral {
</strong>       public static void main(String[] args) {

              byte b = 127;
              System.out.println("byte 變數 b 的值：" + b);
              short s = 32767;
              System.out.println("short 變數 s 的值：" + s);
              int i = 2147483647;
              System.out.println("int 變數 i 的值：" + i);
              long l = 9223372036854775807L;
              System.out.println("long 變數 l 的值：" + l);              

       }
}</code></pre>

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
