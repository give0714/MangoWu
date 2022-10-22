---
description: Informix-4GL 畫面操作說明
---

# WINDOW

## OPEN WINDOW

> ### 自訂視窗大小

```inform7
OPEN WINDOW windowName AT m, n WITH i ROWS, j COLUMNS [ Attribute ]
```

> ### 系統決定視窗大小

```inform7
OPEN WINDOW windowName AT m, n WITH FROM "formFileName"
```

## CURRENT WINDOW

> ### 切換視窗

```inform7
CURRENT WINDOW IS windowName
                  / SCREEN
```

## CLOSE WINDOW

> ### 關閉視窗

```inform7
CLOSE WINDOW windowName
```

## CLEAR WINDOW

> ### 清除所有視窗資訊

```inform7
CLEAR WINDOW
```

{% hint style="info" %}
目的：

清除螢幕所有資訊
{% endhint %}

> ### 清除特定視窗資訊

```inform7
CLEAR WINDOW windowName
```

{% hint style="info" %}
目的：

清除 windowName 上的資訊
{% endhint %}

> ### 清除視窗資訊

```inform7
CLEAR WINDOW SCREEN
```

{% hint style="info" %}
目的：

除 OPEN WINDOW 開啟的資訊保留以外，其餘非上述開啟的所有資訊，將會被清除。
{% endhint %}

## CLEAR fieldList

> ### 清除螢幕欄位資訊

```inform7
CLEAR fieldList
```

{% hint style="info" %}
目的：

清除指定 FORM fieldList 欄位資訊
{% endhint %}

## CLEAR tableName.\*

> ### 清除螢幕相關資料表欄位資訊

```inform7
CLEAR tableName.*
```

{% hint style="info" %}
目的：

清除與指定 tableName 相關的欄位資訊
{% endhint %}

## CLEAR FORMONLY.\*

> ### 清除螢幕與資料表不相關的欄位資訊

```inform7
CLEAR FORMONLY.*
```

{% hint style="info" %}
目的：

清除與資料表無相關的欄位資訊
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
