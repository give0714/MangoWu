---
description: 安裝 Open JDK 流程
---

# 設置 Open JDK

## 步驟 1 \_下載 Open JDK

至網站下載 Open JDK，可至 [openlogic](https://www.openlogic.com/openjdk-downloads)下載。\
<mark style="background-color:green;">推薦使用 JDK 11 來做後續 Java 程式使用。</mark>

## 步驟 2\_安裝 Open JDK

將 Open JDK 解壓縮在硬碟內。

## 步驟 3\_JAVA\_HOME 系統環境變數設定

1. 至 『控制台』->『系統及安全性』->『<mark style="background-color:yellow;">系統</mark>』。
2. 至『系統資訊』->『裝置規格』->『相關連結』->『<mark style="background-color:yellow;">進階系統設定</mark>』。
3. 至『系統內容』->『進階』->『<mark style="background-color:yellow;">環境變數</mark>』。
4. 至『環境變數』->『系統變數』->『<mark style="background-color:yellow;">新增(W)...</mark>』。
5. 在『新增系統變數』內新增下述資訊：
   1. 變數名稱：<mark style="color:red;">JAVA\_HOME</mark>
   2. 變數值：<mark style="background-color:blue;">放置 OpenJDK 的目錄位置</mark>
6. 點選『<mark style="background-color:yellow;">確定</mark>』，此時在系統變數內就會多一個名叫『<mark style="background-color:orange;">JAVA\_HOME</mark>』的系統變數。

## 步驟 4\_PATH 系統環境變數設定

1. 在『環境變數』->『系統變數』，找尋『<mark style="background-color:orange;">Path</mark>』的系統變數，點選兩下並開啟視窗。
2.  在『編輯環境變數』，按下『<mark style="background-color:yellow;">新增(N)</mark>』，並新增下述資訊：

    <mark style="color:red;">%JAVA\_HOME%\bin</mark>
3. 點選新增的『<mark style="background-color:orange;">%JAVA\_HOME%\bin</mark>』欄位，並點選『<mark style="background-color:orange;">上移(U)</mark>』，\
   將該欄位移至第一位後，點選『<mark style="background-color:yellow;">確認</mark>』並關閉視窗。

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有需修改的地方，請前往芒果留言區留言
{% endhint %}
