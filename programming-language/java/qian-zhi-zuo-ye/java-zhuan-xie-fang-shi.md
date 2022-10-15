---
description: Java 撰寫方式說明
---

# Java 撰寫方式

## 檔案副檔名及檔案命名方式

1. 檔案的副檔名為『檔案名稱.java』。
2. 每一個英文字母的第一個字元均為大寫。
3. 檔名需與宣告為 public 的類別同名，大小寫均須相同。

## Java 是區分大小寫 (case sensitive) 組成的語言



## Java 程式是由敘述 ( statements ) 組成的

1. 每行敘述的尾端一定要加分號【 ; 】。
2. 最好一行敘述單獨寫一行。
3. 內縮的編寫方式有利於程式閱讀。

## Java 應用程式主要由類別 ( class ) 組成

1. 所有程式敘述都一定寫在『類別 ( class )』內。

## 類別 ( class ) 主要由方法 ( methon ) 組成

1. 部分程式語言將『方法 ( methin )』稱為『函數 ( function )』。
2. 『main()』 是 Java Application 程式的起點，為第一個被調用的方法。
3. 一般 Java 的敘述都須寫在『方法 ( methin )』內，\
   只有『宣告 ( declarative )』敘述可以寫在方法外。

## Java 的四種註解

1\. 單行註解：

{% code lineNumbers="true" %}
```java
// 註解文字
```
{% endcode %}

2\. 多行註解：

{% code lineNumbers="true" %}
```java
/* 第一行註解文字
   第二行註解文字
   ... */
```
{% endcode %}

3\. 文件註解：

{% code lineNumbers="true" %}
```java
/** 第一行註解文字
    第二行註解文字
    ... */
```
{% endcode %}

4\. Annotation 註解：【JDK 5.0 以後才有的語法】

{% code lineNumbers="true" %}
```java
@Annotation
```
{% endcode %}



{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
