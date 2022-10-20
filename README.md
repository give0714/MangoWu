---
description: 2021-06-23_Company Learning
---

# INFORMIX-4GL

{% hint style="warning" %}
20210816\_持續撰寫中...
{% endhint %}



{% tabs %}
{% tab title="第一章" %}
第一章   變數

1. [宣告變數](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/xuan-gao-bian-shu.md)&#x20;
2. [命名規則](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/untitled.md)
3. [變數初始化](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/bian-shu-chu-shi-hua.md)
4. 變數值設定
   1. [變數不同名的情況](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/bian-shu-fan-wei/bian-shu-bu-tong-ming-de-qing-kuang.md)
   2. [變數同名的情況](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/bian-shu-fan-wei/bian-shu-tong-ming-de-qing-kuang.md)
5. [status 狀態變數](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/status-zhuang-tai-bian-shu.md)
6. [SQLCA系統變數](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/)
   1. [SQLCA.SQLCODE](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlcode.md)
   2. [SQLCA.SQLERRM](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlerrm.md)
   3. [SQLCA.SQLERRP](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlerrp.md)
   4. [SQLCA.SQLERRD](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlerrd.md)
   5. [SQLCA.SQLWARN](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/xi-tong-bian-shu/sqlca.sqlwarn.md)
7. [WHENEVER ERROR 系統錯誤設定](programming-language/mu-ci-biao/di-yi-zhang-bian-shu/whenever-error-xi-tong-cuo-wu-she-ding.md)
{% endtab %}

{% tab title="第二章" %}
第二章   資料型別

1. 簡單資料型別
   1. CHARACTER DATA
      1. [CHAR](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-char-1/jian-chan-zi-liao-xing-bie-char.md)
      2. [VARCHAR](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-char-1/jian-chan-zi-liao-xing-bie-varchar.md)
   2. NUMERIC DATA
      1. [SMALLINT](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-smallint.md)
      2. [INT](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/int.md)
      3. [DECIMAL](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-decimal.md)
      4. [SMALLFLOAT](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-smallfloat.md)
      5. [FLOAT](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/untitled.md)
      6. [MONEY](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-money.md)
      7. [SMALLINT](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-number/jian-chan-zi-liao-xing-bie-smallint.md)
   3. TIME DATA
      1. [DATE](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-time/date.md)
      2. [DATETIME](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-time/datetime.md)
      3. [INTERVAL](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie/jian-chan-zi-liao-xing-bie-time/interval.md)
2. 大型資料型別
   1. [TEXT](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/da-xing-zi-liao-xing-bie/text.md)
   2. [BYTE](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/da-xing-zi-liao-xing-bie/byte.md)
3. 結構資料型別
   1. [RECORD](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jie-gou-zi-liao-xing-bie/record.md)
   2. [ARRAY](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/jie-gou-zi-liao-xing-bie/array.md)
4. 其他資料型別
   1. [SERIAL](programming-language/mu-ci-biao/di-er-zhang-zi-liao-xing-bie/qi-ta-zi-liao-xing-bie/serial.md)
{% endtab %}

{% tab title="第三章" %}
第三章   程式架構

1. [主要架構](programming-language/mu-ci-biao/di-san-zhang/cheng-shi-jia-gou.md)
2. [FUNCTION](programming-language/mu-ci-biao/di-san-zhang/function-han-shu-cheng-shi-jia-gou.md)
3. REPORT
   1. [START REPORT](programming-language/mu-ci-biao/di-san-zhang/report/start-report.md)
   2. [OUTPUT TO REPORT](programming-language/mu-ci-biao/di-san-zhang/report/output-to-report.md)
   3. [FINISH REPORT](programming-language/mu-ci-biao/di-san-zhang/report/finish-report.md)
   4. [REPORT FUNCTION](programming-language/mu-ci-biao/di-san-zhang/report/report-function.md)
   5. REPORT FORMAT Setion
      1. [PRINT](programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/print.md)
      2. [NEED](programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/need.md)
      3. [SKIT](programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/skit.md)
      4. [PAUSE](programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/pause.md)
      5. [EXIT](programming-language/mu-ci-biao/di-san-zhang/report/format-setion-zhi-ling/exit.md)
4. 邏輯判斷敘述
   1. [IF](programming-language/mu-ci-biao/di-san-zhang/luo-ji-pan-duan-xu-shu/if-xu-shu.md)
   2. [FOR](programming-language/mu-ci-biao/di-san-zhang/luo-ji-pan-duan-xu-shu/for-xu-shu.md)
   3. [WHILE](programming-language/mu-ci-biao/di-san-zhang/luo-ji-pan-duan-xu-shu/while-xu-shu.md)
   4. [CASE](programming-language/mu-ci-biao/di-san-zhang/luo-ji-pan-duan-xu-shu/case-xu-shu.md)
   5. [GOTO](programming-language/mu-ci-biao/di-san-zhang/luo-ji-pan-duan-xu-shu/goto-xu-shu.md)
5. [INPUT](programming-language/mu-ci-biao/di-san-zhang/input-xu-shu.md)
6. [INPUT ARRAY](programming-language/mu-ci-biao/di-san-zhang/input-array.md)
{% endtab %}

{% tab title="第四章" %}
第四章   庫存函數

1. 一般型
   1. [ARG\_VAL( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/arg\_val.md)
   2. [NUM\_ARGS( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/num\_args.md)
   3. [SHOWHELP( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/showhelp.md)
   4. [LENGTH( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/length.md)
   5. [ASCII](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/ascii.md)
   6. [ORD( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/ord.md)
   7. [UPSHIFT( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/upshift.md)
   8. [DOWNSHIFT( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/downshift.md)
   9. [USING](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/using.md)
   10. [CLIPPED](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/clipped.md)
   11. [COLUMN](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/column.md)
   12. [SPACE / SPACES](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-yi-ban-xing/space-spaces.md)
2. 陣列型
   1. [SET\_COUNT( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/set\_count.md)
   2. [ARR\_CURR( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/arr\_curr.md)
   3. [SCR\_LINE( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/scr\_line.md)
   4. [INFIELD( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/infield.md)
   5. [GET\_FLDBUF( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/get\_fldbuf.md)
   6. [FIELD\_TOUCHED( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/field\_touched.md)
   7. [ARR\_COUNT( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-zhen-lie-xing/arr\_count.md)
3. 按鍵型
   1. [FGL\_GETKEY( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-an-jian-xing/fgl\_getkey.md)
   2. [FGL\_LASTKEY( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-an-jian-xing/fgl\_lastkey.md)
4. 日期型
   1. [TODAY](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/today.md)
   2. [DATE( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/date.md)
   3. [MDY( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/mdy.md)
   4. [YEAR( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/year.md)
   5. [MONTH( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/month.md)
   6. [DAY( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/day.md)
   7. [WEEKDAY( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/weekday.md)
   8. [TIME](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-ri-qi-xing/time.md)
5. 算術型
   1. [ABS( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/abs.md)
   2. [MOD( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/mod.md)
   3. [COUNT( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/count.md)
   4. [MAX( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/max.md)
   5. [SUM( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/sum.md)
   6. [AVG( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/avg.md)
   7. [RANGE( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-suan-shu-xing/range.md)
6. 錯誤型
   1. [STARTLOG( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-cuo-wu-xing/startlog.md)
   2. [ERR\_PRINT( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-cuo-wu-xing/err\_print.md)
   3. [ERR\_QUIT( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-cuo-wu-xing/err\_quit.md)
   4. [ERR\_GET( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-cuo-wu-xing/err\_get.md)
   5. [ERRORLOG( )](programming-language/mu-ci-biao/di-si-zhang-ku-cun-han-shu/ku-cun-han-shu-cuo-wu-xing/errorlog.md)
{% endtab %}

{% tab title="第五章" %}
第五章   資料庫操作

1. 資料庫操作
   1. [建立資料庫](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-ku-cao-zuo/jian-li-zi-liao-ku.md)
   2. [刪除資料庫](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-ku-cao-zuo/shan-chu-zi-liao-ku.md)
   3. [關閉資料庫](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-ku-cao-zuo/guan-bi-zi-liao-ku.md)
   4. [資料庫連結](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-ku-cao-zuo/zi-liao-ku-lian-jie.md)
   5. 資料庫授權
      1. [CONNECT 權利](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-ku-cao-zuo/zi-liao-ku-shou-quan/connect-quan-li.md)
      2. [RESOURCE 權利](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-ku-cao-zuo/zi-liao-ku-shou-quan/resource-quan-li.md)
      3. [DBA 權利](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-ku-cao-zuo/zi-liao-ku-shou-quan/dba-quan-li.md)
   6. [資料庫命名規則](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-ku-cao-zuo/zi-liao-ku-ming-ming-gui-ze.md)
2. 資料表操作
   1. [建立資料表](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-biao-cao-zuo/jian-li-zi-liao-biao.md)
   2. [資料表更名](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-biao-cao-zuo/zi-liao-biao-geng-ming.md)
   3. [修改資料表儲存空間](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-biao-cao-zuo/xiu-gai-zi-liao-biao-chu-cun-kong-jian.md)
   4. [修改資料表鎖定程度](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-biao-cao-zuo/xiu-gai-zi-liao-biao-suo-ding-cheng-du.md)
   5. [刪除資料表](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-biao-cao-zuo/shan-chu-zi-liao-biao.md)
   6. [資料表授權](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-biao-cao-zuo/zi-liao-biao-shou-quan.md)
   7. [資料表命名規則](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/zi-liao-biao-cao-zuo/zi-liao-biao-ming-ming-gui-ze.md)
3. 欄位操作
   1. [新增欄位](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/lan-wei-cao-zuo/xin-zeng-lan-wei.md)
   2. [新增欄位屬性](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/lan-wei-cao-zuo/xin-zeng-lan-wei-shu-xing.md)
   3. [欄位更名](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/lan-wei-cao-zuo/lan-wei-geng-ming.md)
   4. [修改欄位](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/lan-wei-cao-zuo/xiu-gai-lan-wei.md)
   5. [刪除欄位](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/lan-wei-cao-zuo/shan-chu-lan-wei.md)
   6. [刪除欄位屬性](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/lan-wei-cao-zuo/shan-chu-lan-wei-shu-xing.md)
   7. [欄位命名規則](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/lan-wei-cao-zuo/lan-wei-ming-ming-gui-ze.md)
4. 索引操作
   1. [索引說明](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/suo-yin-cao-zuo/suo-yin-shuo-ming.md)
   2. [建立索引](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/suo-yin-cao-zuo/jian-li-suo-yin.md)
   3. [修改索引 CLUSTER 狀態](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/suo-yin-cao-zuo/xiu-gai-suo-yin-cluster-zhuang-tai.md)
   4. [刪除索引](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/suo-yin-cao-zuo/shan-chu-suo-yin.md)
   5. [索引命名規則](programming-language/mu-ci-biao/di-wu-zhang-zi-liao-ku-cao-zuo-ji-shou-quan/suo-yin-cao-zuo/suo-yin-ming-ming-gui-ze.md)
{% endtab %}

{% tab title="第六章" %}
第六章   資料處理

1. SQL Language
   1. [INSERT 語法](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/sql-language/insert-yu-fa.md#yu-fa)
   2. [DELETE 語法](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/sql-language/delete-yu-fa.md#yu-fa)
   3. [UPDATE 語法](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/sql-language/update-yu-fa.md#yu-fa-yi)
   4. [SELECT 語法](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/sql-language/select-yu-fa.md#yu-fa)
2. [SQL ... END SQL](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/sql-...-end-sql.md#yu-fa)
3. CURSOR
   1. [CURSOR 使用方法](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/cursor/cursor-shi-yong-fang-shi.md)
   2. [SCROLL CURSOR](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/cursor/scroll-cursor.md)
   3. [一般 CURSOR](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/cursor/yi-ban-cursor.md)
   4. [INSERT 操作](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/cursor/insert-cao-zuo.md#yu-fa)
   5. [UPDATE 操作](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/cursor/update-cao-zuo.md#yu-fa)
   6. SELECT 操作
      1. [人工手動控制游標](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/cursor/select-cao-zuo/ren-gong-shou-dong-kong-zhi-you-biao.md#yu-fa)
      2. [系統自動控制游標](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/cursor/select-cao-zuo/xi-tong-zi-dong-kong-zhi-you-biao.md#yu-fa)
4. [QBE](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/qbe.md)
5. [CONSTRUCT](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/construct.md)
6. [Transaction](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/transaction.md)
7. [補充內容](programming-language/mu-ci-biao/di-liu-zhang-zi-liao-cao-zuo-ji-jiao-yi-chu-li/bu-chong-nei-rong.md)
{% endtab %}

{% tab title="第七章" %}
第七章   FORM 及 WINDOW

1.
{% endtab %}
{% endtabs %}



{% hint style="danger" %}
【 M@nGo 留言區 】\
如有任何建議的地方，請前往芒果留言區留言
{% endhint %}
