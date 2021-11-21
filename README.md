---
description: 2021-06-23_Company Learning
---

# INFORMIX-4GL

{% hint style="warning" %}
20210816\_持續撰寫中...
{% endhint %}

{% tabs %}
{% tab title="第一章" %}
第一章\_變數

1. [宣告變數](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/xuan-gao-bian-shu.md)&#x20;
2. [命名規則](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/untitled.md)
3. [變數初始化](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/bian-shu-chu-shi-hua.md)
4. 變數值設定
   1. [變數不同名的情況](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/bian-shu-fan-wei/bian-shu-bu-tong-ming-de-qing-kuang.md)
   2. [變數同名的情況](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/bian-shu-fan-wei/bian-shu-tong-ming-de-qing-kuang.md)
5. [status 狀態變數](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/status-zhuang-tai-bian-shu.md)
6. [SQLCA系統變數](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/)
   1. [SQLCA.SQLCODE](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlcode.md)
   2. [SQLCA.SQLERRM](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlerrm.md)
   3. [SQLCA.SQLERRP](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlerrp.md)
   4. [SQLCA.SQLERRD](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlerrd.md)
   5. [SQLCA.SQLWARN](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlwarn.md)
7. [WHENEVER ERROR 系統錯誤設定](informix-4gl-learning/mu-ci-biao/di-yi-zhang-bian-shu/whenever-error-xi-tong-cuo-wu-she-ding.md)
{% endtab %}

{% tab title="第二章" %}
第二章\_資料型別

1. 簡單資料型別
   1. CHARACTER DATA
      1. [CHAR](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-char-1/jian-chan-zi-liao-xing-bie-char.md)
      2. [VARCHAR](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-char-1/jian-chan-zi-liao-xing-bie-varchar.md)
   2. NUMERIC DATA
      1. [SMALLINT](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-smallint.md)
      2. [INT](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/int.md)
      3. [DECIMAL](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-decimal.md)
      4. [SMALLFLOAT](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-smallfloat.md)
      5. [FLOAT](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/untitled.md)
      6. [MONEY](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-money.md)
      7. [SMALLINT](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-smallint.md)
   3. TIME DATA
      1. [DATE](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-time/date.md)
      2. [DATETIME](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-time/datetime.md)
      3. [INTERVAL](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-time/interval.md)
2. 大型資料型別
   1. [TEXT](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/da-xing-zi-liao-xing-bie/text.md)
   2. [BYTE](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/da-xing-zi-liao-xing-bie/byte.md)
3. 結構資料型別
   1. [RECORD](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jie-gou-zi-liao-xing-bie/record.md)
   2. [ARRAY](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jie-gou-zi-liao-xing-bie/array.md)
4. 其他資料型別
   1. [SERIAL](informix-4gl-learning/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/qi-ta-zi-liao-xing-bie/serial.md)
{% endtab %}

{% tab title="第三章" %}
第三章\_程式架構

1. [主要架構](informix-4gl-learning/mu-ci-biao/di-san-zhang/cheng-shi-jia-gou.md)
2. [FUNCTION](informix-4gl-learning/mu-ci-biao/di-san-zhang/function-han-shu-cheng-shi-jia-gou.md)
3. REPORT
   1. [START REPORT](informix-4gl-learning/mu-ci-biao/di-san-zhang/report/start-report.md)
   2. [OUTPUT TO REPORT](informix-4gl-learning/mu-ci-biao/di-san-zhang/report/output-to-report.md)
   3. [FINISH REPORT](informix-4gl-learning/mu-ci-biao/di-san-zhang/report/finish-report.md)
   4. [REPORT FUNCTION](informix-4gl-learning/mu-ci-biao/di-san-zhang/report/report-function.md)
   5. REPORT FORMAT Setion
      1. [PRINT](programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/print.md)
      2. [NEED](programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/need.md)
      3. [SKIT](programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/skit.md)
      4. [PAUSE](programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/pause.md)
      5. [EXIT](programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/exit.md)
4. 邏輯判斷敘述
   1. [IF](informix-4gl-learning/mu-ci-biao/di-san-zhang/luo-ji-pan-duan-xu-shu/if-xu-shu.md)
   2. [FOR](informix-4gl-learning/mu-ci-biao/di-san-zhang/luo-ji-pan-duan-xu-shu/for-xu-shu.md)
   3. [WHILE](informix-4gl-learning/mu-ci-biao/di-san-zhang/luo-ji-pan-duan-xu-shu/while-xu-shu.md)
   4. [CASE](informix-4gl-learning/mu-ci-biao/di-san-zhang/luo-ji-pan-duan-xu-shu/case-xu-shu.md)
   5. [GOTO](informix-4gl-learning/mu-ci-biao/di-san-zhang/luo-ji-pan-duan-xu-shu/goto-xu-shu.md)
5. [INPUT](informix-4gl-learning/mu-ci-biao/di-san-zhang/input-xu-shu.md)
6. [INPUT ARRAY](informix-4gl-learning/mu-ci-biao/di-san-zhang/input-array.md)
{% endtab %}

{% tab title="第四章" %}
第四章\_庫存函數

1. 一般型
   1. [ARG\_VAL( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/arg\_val.md)
   2. [NUM\_ARGS( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/num\_curr.md)
   3. [SHOWHELP( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/showhelp.md)
   4. [LENGTH( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/length.md)
   5. [ASCII](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/ascii.md)
   6. [ORD( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/ord.md)
   7. [UPSHIFT( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/upshift.md)
   8. [DOWNSHIFT( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/downshift.md)
   9. [USING](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/using.md)
   10. [CLIPPED](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/clipped.md)
   11. [COLUMN](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/column.md)
   12. [SPACE / SPACES](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/space-spaces.md)
2. 陣列型
   1. [SET\_COUNT( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/set\_count.md)
   2. [ARR\_CURR( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/arr\_curr.md)
   3. [SCR\_LINE( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/scr\_line.md)
   4. [INFIELD( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/infield.md)
   5. [GET\_FLDBUF( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/get\_fldbuf.md)
   6. [FIELD\_TOUCHED( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/field\_touched.md)
   7. [ARR\_COUNT( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/arr\_count.md)
3. 按鍵型
   1. [FGL\_GETKEY( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-an-jian-xing/fgl\_getkey.md)
   2. [FGL\_LASTKEY( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-an-jian-xing/fgl\_lastkey.md)
4. 日期型
   1. [TODAY](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/today.md)
   2. [DATE( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/date.md)
   3. [MDY( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/mdy.md)
   4. [YEAR( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/year.md)
   5. [MONTH( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/month.md)
   6. [DAY( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/day.md)
   7. [WEEKDAY( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/weekday.md)
   8. [TIME](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/time.md)
5. 算術型
   1. [ABS( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/abs.md)
   2. [MOD( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/mod.md)
   3. [COUNT( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/count.md)
   4. [MAX( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/max.md)
   5. [SUM( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/sum.md)
   6. [AVG( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/avg.md)
   7. [RANGE( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/range.md)
6. 錯誤型
   1. [STARTLOG( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/startlog.md)
   2. [ERR\_PRINT( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-cuo-wu-xing/err\_print.md)
   3. [ERR\_QUIT( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-cuo-wu-xing/err\_quit.md)
   4. [ERR\_GET( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-cuo-wu-xing/err\_get.md)
   5. [ERRORLOG( )](informix-4gl-learning/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-cuo-wu-xing/errorlog.md)
{% endtab %}

{% tab title="第五章" %}
第五章\_資料庫操作 及 授權

1.
{% endtab %}

{% tab title="第六章" %}
第六章\_資料處理

1.
{% endtab %}

{% tab title="第七章" %}
第七章\_交易處理

1.
{% endtab %}

{% tab title="第八章" %}
第八章\_FORM 及 WINDOW

1.
{% endtab %}
{% endtabs %}

{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言
{% endhint %}
