---
description: Informix-4GL 報表架構說明《五》
---

# PRINT

## 語法

```objectivec
PRINT
      [ 4GL_Statement ]
      [ COLUMN num ]
      [ PAGENO ]
      [ LINENO ]
      [ BYTE variable ]
      [ mathStatement ( SPACE / SPACES ) ]
      [[ GROUP ] ( PERCENT(*)
                   / COUNT(*)
                   / AVG( integerStatement / 區間 statement )
                   / SUM( integerStatement / 區間 statement )
                   / MAX( 4GL_Statement )
                   / MIM( 4GL_Statement )                     )
                 [ WHERE BOOLEAN statement ]                    ]
      [ charStatement / charVariable [ WORDWRAP ][ RIGHT MARGIN num ] ]
      [ FILE "fileName" ]
                   
```

{% hint style="info" %}
目的

設定輸出格式。
{% endhint %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言。
{% endhint %}
