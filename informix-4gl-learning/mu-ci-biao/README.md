---
description: 2021-06-23_Company Learning
---

# INFORMIX-4GL

{% hint style="warning" %}
20210816\_持續撰寫中...
{% endhint %}

{% tabs %}
{% tab title="一" %}
第一章變數

1. [宣告變數](di-yi-zhang-bian-shu/xuan-gao-bian-shu.md)&#x20;
2. [命名規則](di-yi-zhang-bian-shu/untitled.md)
3. [變數初始化](di-yi-zhang-bian-shu/bian-shu-chu-shi-hua.md)
4. 變數值設定
   1. [變數不同名的情況](di-yi-zhang-bian-shu/bian-shu-fan-wei/bian-shu-bu-tong-ming-de-qing-kuang.md)
   2. [變數同名的情況](di-yi-zhang-bian-shu/bian-shu-fan-wei/bian-shu-tong-ming-de-qing-kuang.md)
5. [status 狀態變數](di-yi-zhang-bian-shu/status-zhuang-tai-bian-shu.md)
6. [SQLCA系統變數](di-yi-zhang-bian-shu/xi-tong-bian-shu/)
   1. [SQLCA.SQLCODE](di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlcode.md)
   2. [SQLCA.SQLERRM](di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlerrm.md)
   3. [SQLCA.SQLERRP](di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlerrp.md)
   4. [SQLCA.SQLERRD](di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlerrd.md)
   5. [SQLCA.SQLWARN](di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlwarn.md)
7. [WHENEVER ERROR 系統錯誤設定](di-yi-zhang-bian-shu/whenever-error-xi-tong-cuo-wu-she-ding.md)
{% endtab %}

{% tab title="二" %}
第二章資料型別

1. 簡單資料型別
   1. CHARACTER DATA
      1. [CHAR](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-char-1/jian-chan-zi-liao-xing-bie-char.md)
      2. [VARCHAR](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-char-1/jian-chan-zi-liao-xing-bie-varchar.md)
   2. NUMERIC DATA
      1. [SMALLINT](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-smallint.md)
      2. [INT](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/int.md)
      3. [DECIMAL](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-decimal.md)
      4. [SMALLFLOAT](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-smallfloat.md)
      5. [FLOAT](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/untitled.md)
      6. [MONEY](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-money.md)
      7. [SMALLINT](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-smallint.md)
   3. TIME DATA
      1. [DATE](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-time/date.md)
      2. [DATETIME](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-time/datetime.md)
      3. [INTERVAL](di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-time/interval.md)
2. 大型資料型別
   1. [TEXT](di-er-zhang-zi-liao-xing-bie/da-xing-zi-liao-xing-bie/text.md)
   2. [BYTE](di-er-zhang-zi-liao-xing-bie/da-xing-zi-liao-xing-bie/byte.md)
3. 結構資料型別
   1. [RECORD](di-er-zhang-zi-liao-xing-bie/jie-gou-zi-liao-xing-bie/record.md)
   2. [ARRAY](di-er-zhang-zi-liao-xing-bie/jie-gou-zi-liao-xing-bie/array.md)
4. 其他資料型別
   1. [SERIAL](di-er-zhang-zi-liao-xing-bie/qi-ta-zi-liao-xing-bie/serial.md)
{% endtab %}

{% tab title="三" %}
第三章程式架構

1. [主要架構](di-san-zhang/cheng-shi-jia-gou.md)
2. [FUNCTION](di-san-zhang/function-han-shu-cheng-shi-jia-gou.md)
3. REPORT
   1. [START REPORT](di-san-zhang/report/start-report.md)
   2. [OUTPUT TO REPORT](di-san-zhang/report/output-to-report.md)
   3. [FINISH REPORT](di-san-zhang/report/finish-report.md)
   4. [REPORT FUNCTION](di-san-zhang/report/report-function.md)
   5. REPORT FORMAT Setion
      1. [PRINT](../../programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/print.md)
      2. [NEED](../../programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/need.md)
      3. [SKIT](../../programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/skit.md)
      4. [PAUSE](../../programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/pause.md)
      5. [EXIT](../../programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/exit.md)
4. 邏輯判斷敘述
   1. [IF](di-san-zhang/luo-ji-pan-duan-xu-shu/if-xu-shu.md)
   2. [FOR](di-san-zhang/luo-ji-pan-duan-xu-shu/for-xu-shu.md)
   3. [WHILE](di-san-zhang/luo-ji-pan-duan-xu-shu/while-xu-shu.md)
   4. [CASE](di-san-zhang/luo-ji-pan-duan-xu-shu/case-xu-shu.md)
   5. [GOTO](di-san-zhang/luo-ji-pan-duan-xu-shu/goto-xu-shu.md)
5. [INPUT](di-san-zhang/input-xu-shu.md)
6. [INPUT ARRAY](di-san-zhang/input-array.md)
{% endtab %}

{% tab title="四" %}
第四章庫存函數

1.
{% endtab %}

{% tab title="五" %}
第五章\_

1.
{% endtab %}

{% tab title="六" %}
第六章\_

1.
{% endtab %}

{% tab title="七" %}
第七章\_

1.
{% endtab %}
{% endtabs %}

