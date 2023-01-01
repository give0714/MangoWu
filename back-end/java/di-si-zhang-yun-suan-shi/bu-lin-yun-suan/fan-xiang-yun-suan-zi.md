---
description: Java 運算式說明章節
---

# 反向運算子

## 反向運算子 Logical Complement Operator

### 種類

* ! var

{% code title="Complement.java" lineNumbers="true" %}
```java
public class Complement {

	public static void main(String[] args) {
		
		boolean b = false;
		System.out.println("現在是否有開燈 ?");
		lightOpen(b);
		System.out.println("現在關了嗎 ?");
		lightOpen(!b);

	}
	
	public static void lightOpen(boolean var) {
		
		if (var) {
			System.out.println("有關燈了~~");
		} else {
			System.out.println("沒有關燈!!");
			System.out.println("請關閉電源");
		}		
		
	}

}
```
{% endcode %}

{% code title="執行結果" %}
```
現在是否有開燈 ?
沒有關燈!!
請關閉電源
現在關了嗎 ?
有關燈了~~
```
{% endcode %}

{% hint style="info" %}
備註：

* 只能用於變數，無法用於常數或算式。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
