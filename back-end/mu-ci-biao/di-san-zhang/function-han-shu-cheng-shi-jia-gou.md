---
description: Informix-4GL 函數架構說明
---

# FUNCTION

## 呼叫函數

```objectivec
CALL functionName( { transferVariableName1 
                  {, transferVariableName2
                   , ... }} )
   [ RETURNING returnVariableName1 
            {, returnVariableName2
             , ... } ]
```

## 執行函數

```objectivec
FUNCTION functionName( { transferVariableName1
                      {, transferVariableName2
                       , ... }} )
         ...
       [ RETURN returnVariableName1
             {, returnVariableName2
              , ... } ]
END FUNCTION
```

{% hint style="info" %}
說明

* 傳遞參數\_transferVariableName：\
  為程式傳遞至函數的參數\
  除了參數的資料型別不能為 ARRAY 型別及 RECORD.\* 型別外，其他的資料型別均可使用\
  使用前，須於 CALL 敘述前宣告承接參數的變數及其屬性\
  參數可傳可不傳，也可傳遞一個含以上的參數，但 CALL 與 FUNCTION 之間傳遞及承接的參數數量及屬性均需一致\

* 回傳參數\_returnVariableName：\
  為函數傳遞至程式的參數\
  除了參數的資料型別不能為 ARRAY 型別及含 ARRAY 型別的 RECORD 型別，其他的資料型別均可使用\
  使用前，須於 CALL 敘述前宣告承接參數的變數及其屬性\
  參數可傳可不傳，也可傳遞一個含以上的參數，但 CALL 與 FUNCTION 之間傳遞及承接的參數數量及屬性均需一致
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
