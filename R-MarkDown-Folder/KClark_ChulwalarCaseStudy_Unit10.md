Import Data for Chulwahlar Forecasting Exports
==============================================

Preparing for Import
--------------------

    ## Loading required package: forecast

    ## Loading required package: zoo

    ## 
    ## Attaching package: 'zoo'

    ## The following objects are masked from 'package:base':
    ## 
    ##     as.Date, as.Date.numeric

    ## Loading required package: timeDate

    ## This is forecast 7.1

    ## Loading required package: fma

    ## Loading required package: tseries

    ## Loading required package: expsmooth

    ## Loading required package: lmtest

Import Data set
===============

Imported the Observed data set (ImportedAsIsDataChulwalar.csv)

Imported the Plan Data set (ImportedPlanDataChulwalar.csv)

Imported the Indicator Data Set (ImportedIndicatorsChulwalar.csv)

Data Transformations
====================

Data Vectors were created with partial data sets for data analysis and
forecasting.

As Is Data Set Vectors Created:

1.  TotalAsIsVector
2.  TotalEtelAsIsVector
3.  BlueEtelAsIsVector
4.  RedEtelAsIsVector
5.  YearAsIsVector
6.  TotalAsIsVector\_2014

Plan Data Vectors Created:

1.  PlanVector
2.  TotalEtelPlanVector
3.  BlueEtelPlanVector
4.  RedEtelPlanVector
5.  YearPlanVector
6.  PlanVector\_2014

The Vectors were then converted into Time Series data sets.

Below is a review of the time series data sets created for the following
Total As Is Data, Total Etel Flower As Is, Blue Etel Flower As Is, Red
Etel Flower As IS, Year As IS, and Total As Is for 2014.

Total As Is:

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2008 2313221 1950131 2346635 2039787 1756964 1458302 1679637 1639670
    ## 2009 2610573 2371327 2743786 2125308 1850073 1836222 1797311 1851968
    ## 2010 2760688 2918333 3227041 1613888 2550157 2317645 1474144 2148521
    ## 2011 3112861 2926663 3294784 2577079 2774068 2378227 2222900 2991787
    ## 2012 3093088 3679308 3433364 2714899 3011767 2726028 2483834 3055655
    ## 2013 4119526 3535744 3560974 3760065 2959933 2787898 2828744 3084113
    ##          Sep     Oct     Nov     Dec
    ## 2008 2882886 2959716 2596494 2656568
    ## 2009 3271171 2818888 3310776 3022513
    ## 2010 3898571 3348953 3135945 3332886
    ## 2011 4151531 3318684 4037076 3429843
    ## 2012 4200796 4228724 4618540 3383673
    ## 2013 5107775 4562144 4729313 4372181

Total Etel Flower As Is:

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2008 1279668 1053325 1367520 1090725  873568  644479  772658  806741
    ## 2009 1583216 1407388 1420801 1141100  919860  858876  910134  843050
    ## 2010 1637464 1676161 1549560  813469 1198401 1140024  551268 1012542
    ## 2011 1595267 1473528 1469728 1034650  952553  819303  802076 1222812
    ## 2012 1519748 1812897 1607280 1008022 1291983  940158  945929 1235146
    ## 2013 2109497 1738197 1633944 1745092 1039449 1054201 1003166 1154675
    ##          Sep     Oct     Nov     Dec
    ## 2008 1715265 1795751 1518288 1601324
    ## 2009 1981563 1647934 1857836 1615091
    ## 2010 2335488 1856264 1678123 1699063
    ## 2011 2303271 1591584 1960675 1713991
    ## 2012 2330334 2177895 2306324 1618147
    ## 2013 3000929 2305605 2284672 2062160

Blue Etel Flower As Is:

    ##         Jan    Feb    Mar    Apr    May    Jun    Jul    Aug    Sep    Oct
    ## 2008 425892 316631 353512 278711 212940 187849 206285 195810 448733 403327
    ## 2009 407424 287654 305158 255687 200068 210118 211668 198472 361703 366410
    ## 2010 369783 345144 322695 223841 239441 240316 138604 231179 329090 368584
    ## 2011 308893 282106 347124 261498 217606 208258 174878 247714 312012 331926
    ## 2012 285207 450874 360034 252674 247734 221676 216918 254993 299658 457595
    ## 2013 387497 349013 334274 325052 255416 237019 239047 358552 359703 427681
    ##         Nov    Dec
    ## 2008 306171 345955
    ## 2009 350196 351651
    ## 2010 320947 373302
    ## 2011 389858 299115
    ## 2012 388917 303450
    ## 2013 434561 348558

Red Etel Flower As Is:

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2008  853776  736694 1014008  812014  660628  456630  566373  610931
    ## 2009 1175792 1119734 1115643  885413  719792  648758  698466  644578
    ## 2010 1267682 1331017 1226866  589628  958960  899709  412664  781363
    ## 2011 1286374 1191422 1122604  773151  734947  611045  627198  975098
    ## 2012 1234541 1362023 1247246  755347 1044249  718482  729011  980154
    ## 2013 1722000 1389184 1299670 1420039  784033  817182  764120  796123
    ##          Sep     Oct     Nov     Dec
    ## 2008 1266532 1392424 1212117 1255369
    ## 2009 1619860 1281524 1507640 1263440
    ## 2010 2006398 1487680 1357176 1325761
    ## 2011 1991259 1259658 1570817 1414876
    ## 2012 2030676 1720301 1917408 1314697
    ## 2013 2641226 1877924 1850111 1713603

Year As Is:

    ##           Jan      Feb      Mar      Apr      May      Jun      Jul
    ## 2008 26280011 29609916 32726772 37215503 40629676 45408410 26280011
    ## 2009 26280011 29609916 32726772 37215503 40629676 45408410 26280011
    ## 2010 26280011 29609916 32726772 37215503 40629676 45408410 26280011
    ## 2011 26280011 29609916 32726772 37215503 40629676 45408410 26280011
    ## 2012 26280011 29609916 32726772 37215503 40629676 45408410 26280011
    ## 2013 26280011 29609916 32726772 37215503 40629676 45408410 26280011
    ##           Aug      Sep      Oct      Nov      Dec
    ## 2008 29609916 32726772 37215503 40629676 45408410
    ## 2009 29609916 32726772 37215503 40629676 45408410
    ## 2010 29609916 32726772 37215503 40629676 45408410
    ## 2011 29609916 32726772 37215503 40629676 45408410
    ## 2012 29609916 32726772 37215503 40629676 45408410
    ## 2013 29609916 32726772 37215503 40629676 45408410

Total As Is 2014:

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2014 4308161 4155378 3924332 3659121 3898758 3313891 3595106 3502426
    ##          Sep     Oct     Nov     Dec
    ## 2014 5619059 5274287 4841693 4664854

Below is a review of the time series data sets created for the following
Total Plan, Total Etel Flower Plan, Blue Etel Flower Plan, Red Etel
Flower Plan, Year Plan, and Total Plan for 2014.

Total Plan:

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2008 2243103 2162705 2720911 2011182 1877757 1819924 1682196 1893171
    ## 2009 2547980 2247049 2731156 2020158 2098038 1927995 1783692 1907705
    ## 2010 2965885 2751170 2906493 2383358 2246893 1992851 2023434 2244997
    ## 2011 3113110 2883766 2957893 2601648 2370949 2339881 2105328 2341623
    ## 2012 3895396 3588151 3787240 3036434 2907891 2707822 2619486 3784557
    ## 2013 3580325 3863212 3606083 3213575 3139128 2998610 2785453 3083654
    ##          Sep     Oct     Nov     Dec
    ## 2008 3325711 2662148 2909966 2574633
    ## 2009 3124040 3102251 3154669 2742367
    ## 2010 3257717 3536338 3358206 3112906
    ## 2011 4086297 3640827 3502334 3280476
    ## 2012 4987460 4367319 4205772 4059533
    ## 2013 5143757 4149334 4495212 4093664

Total Etel Flower Plan:

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2008 1263613 1231125 1489621 1051346  933392  932047  855520  923070
    ## 2009 1546801 1378217 1563799 1166229 1057223  983279  913751  980703
    ## 2010 1648769 1490577 1538493 1208636 1104777  931127  916160 1096933
    ## 2011 1781991 1564272 1455531 1257528 1134418 1018200  843336  974375
    ## 2012 2070256 1731099 1663266 1232994 1164076 1018137  932241 1800576
    ## 2013 1864733 1837228 1663834 1305603 1172373 1089115 1074687 1217930
    ##          Sep     Oct     Nov     Dec
    ## 2008 2080877 1575579 1561956 1515127
    ## 2009 1974166 1886971 1839155 1727567
    ## 2010 1832882 2103588 1877929 1862684
    ## 2011 2435674 1972649 1873075 1684766
    ## 2012 2823873 2224655 2025003 1955509
    ## 2013 2916115 2043888 2199880 2133214

Blue Etel Flower Plan:

    ##         Jan    Feb    Mar    Apr    May    Jun    Jul    Aug    Sep    Oct
    ## 2008 449227 373663 415732 331337 290942 287603 245390 284540 554127 467772
    ## 2009 394188 320490 351375 271021 225914 234600 191342 226507 519935 512283
    ## 2010 388677 317587 306376 275940 235850 224371 204869 220570 357203 413862
    ## 2011 412463 323577 313230 276210 249768 217911 209229 219002 365415 421679
    ## 2012 481147 412798 364106 311291 283279 286839 249233 288342 399167 524838
    ## 2013 360982 342370 346868 277548 251623 257153 232752 252611 494843 445720
    ##         Nov    Dec
    ## 2008 469089 409962
    ## 2009 456203 376595
    ## 2010 357645 364243
    ## 2011 359800 343171
    ## 2012 399038 415564
    ## 2013 414612 401854

Red Etel Flower Plan;

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2008  814386  857462 1073889  720009  642450  644444  610130  638530
    ## 2009 1152613 1057727 1212424  895208  831309  748679  722409  754196
    ## 2010 1260092 1172990 1232117  932696  868927  706756  711291  876363
    ## 2011 1369528 1240695 1142301  981318  884650  800289  634107  755372
    ## 2012 1589109 1318301 1299159  921703  880796  731299  683008 1512234
    ## 2013 1503751 1494858 1316966 1028055  920750  831961  841936  965319
    ##          Sep     Oct     Nov     Dec
    ## 2008 1526750 1107807 1092867 1105165
    ## 2009 1454231 1374688 1382952 1350972
    ## 2010 1475679 1689726 1520284 1498441
    ## 2011 2070259 1550970 1513274 1341595
    ## 2012 2424705 1699817 1625965 1539945
    ## 2013 2421272 1598167 1785268 1731360

Year Plan:

    ##           Jan      Feb      Mar      Apr      May      Jun      Jul
    ## 2008 27883407 29387100 32780247 35224132 43947063 44152007 27883407
    ## 2009 27883407 29387100 32780247 35224132 43947063 44152007 27883407
    ## 2010 27883407 29387100 32780247 35224132 43947063 44152007 27883407
    ## 2011 27883407 29387100 32780247 35224132 43947063 44152007 27883407
    ## 2012 27883407 29387100 32780247 35224132 43947063 44152007 27883407
    ## 2013 27883407 29387100 32780247 35224132 43947063 44152007 27883407
    ##           Aug      Sep      Oct      Nov      Dec
    ## 2008 29387100 32780247 35224132 43947063 44152007
    ## 2009 29387100 32780247 35224132 43947063 44152007
    ## 2010 29387100 32780247 35224132 43947063 44152007
    ## 2011 29387100 32780247 35224132 43947063 44152007
    ## 2012 29387100 32780247 35224132 43947063 44152007
    ## 2013 29387100 32780247 35224132 43947063 44152007

Total Plan for 2014:

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2014 4474000 4185565 4278119 3985542 3605973 3515173 3269444 3656112
    ##          Sep     Oct     Nov     Dec
    ## 2014 5637391 5157781 5353458 4703185

Data Analysis on the Blue Etel Flower
=====================================

Plots of As Is data:
--------------------

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-20-1.png)<!-- -->

The Blue Etel sales account for a large majority of the Etel flower
sales. The Red Etel had greater sales in 2014 where the Blue Etel
faltered. The sales plot displays seasonality. Sales appear to have
dropped drastically between 2010 and 2011 for all Etel flowers and could
possibly account for weather or a bad growth season.

Plots of Plan Data:
-------------------

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-21-1.png)<!-- -->

Since the basic plots of the Etel flowers that separate seasonality and
trend. Below are some plots that examine the seasonality a little more
in depth but add trending. The remainder graph basically identifies any
noise in the data that might skew the seasonality or trend data.

The plots below are based on the time series data sets instead of the
current data data sets.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-23-1.png)<!-- -->

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-24-1.png)<!-- -->

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-25-1.png)<!-- -->

When viewing the overall Etel Flower Exports by seasonal and inherit
trends, you can see that the seasonal panel is only slightly larger than
that on the data panel, which indicates the seasonal signal is largely
relative to the variation in the data. When looking at the trend plot it
is much larger than the seasonal plot, which indicates the variation
attributed to the trend is much smaller than the seasonal component. The
overall export data of both Etel flowers and each individual flower plot
does not exhibit a trend.

Modify the Seasonal data to view it at a monthly level
------------------------------------------------------

Even though the above plots do not indicate that the seasonal and trend
plot look identical, breaking the data down by month will an alternative
view.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-26-1.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-26-2.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-26-3.png)<!-- -->

All three plots display a drop in exports in July and a sharp increase
in exports in September. The monthly plots do display a trend associated
with seasonality that is driven by the temperature in Chulwalar.

Viewing Correlations between the As Is data and the Plan:
---------------------------------------------------------

Correlation between the Total As Is data and the Total Plan:

    ## [1] 0.9183402

Correlation between the Total Etel Flower As Is data and the Total Etel
Plan:

    ## [1] 0.9159505

Correlation between the Total Blue Etel Flower As Is data and the Total
Blue Etel Plan:

    ## [1] 0.8044146

Correlation between the Total Red Etel Flower As Is data and the Total
Red Etel Plan:

    ## [1] 0.9106702

There is a strong correlation between the current As Is data for the
Etel flower and the plan data for the Etel Flower. The Blue Etel flower
As Is data and Plan correlation is not as strong as the Red Etel
flowers.

View the Differences between the As Is data and the Plan data
-------------------------------------------------------------

This analysis is to make sure the plan is accurate and that the data is
identical.

View of the Total As Is differences:

    ## 
    ## Call:
    ## lm(formula = TotalAsIs ~ TotalPlan, data = TotalAsIs)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -770214 -196776   26017  182579  672705 
    ## 
    ## Coefficients:
    ##              Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept) 8.959e+04  1.521e+05   0.589    0.558    
    ## TotalPlan   9.627e-01  4.959e-02  19.413   <2e-16 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 332600 on 70 degrees of freedom
    ## Multiple R-squared:  0.8433, Adjusted R-squared:  0.8411 
    ## F-statistic: 376.9 on 1 and 70 DF,  p-value: < 2.2e-16

View of the Total As Is Time Series data differences

    ## 
    ## Call:
    ## tslm(formula = TotalAsIs ~ TotalPlan)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -770214 -196776   26017  182579  672705 
    ## 
    ## Coefficients:
    ##              Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept) 8.959e+04  1.521e+05   0.589    0.558    
    ## TotalPlan   9.627e-01  4.959e-02  19.413   <2e-16 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 332600 on 70 degrees of freedom
    ## Multiple R-squared:  0.8433, Adjusted R-squared:  0.8411 
    ## F-statistic: 376.9 on 1 and 70 DF,  p-value: < 2.2e-16

The As Is data and the As Is Time Series data match the plan data. The
adjusted R square for both equal 0.8411.

View the Total Etel Flower As Is Data:

    ## 
    ## Call:
    ## lm(formula = TotalEtelAsIs ~ TotalEtelPlan, data = TotalEtelAsIs)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -492888  -99871   -7667   93858  576321 
    ## 
    ## Coefficients:
    ##                 Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)   -7.175e+03  8.018e+04  -0.089    0.929    
    ## TotalEtelPlan  9.637e-01  5.046e-02  19.097   <2e-16 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 202900 on 70 degrees of freedom
    ## Multiple R-squared:  0.839,  Adjusted R-squared:  0.8367 
    ## F-statistic: 364.7 on 1 and 70 DF,  p-value: < 2.2e-16

The Etel Flower As Is data and the Etel Flower As Is Time Series data
match the plan data for the Etel Flower. The adjusted R square for both
equal 0.8367.

View the Total Etel Flower As Is Time Series data Differences:

    ## 
    ## Call:
    ## tslm(formula = TotalEtelAsIs ~ TotalEtelPlan)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -492888  -99871   -7667   93858  576321 
    ## 
    ## Coefficients:
    ##                 Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)   -7.175e+03  8.018e+04  -0.089    0.929    
    ## TotalEtelPlan  9.637e-01  5.046e-02  19.097   <2e-16 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 202900 on 70 degrees of freedom
    ## Multiple R-squared:  0.839,  Adjusted R-squared:  0.8367 
    ## F-statistic: 364.7 on 1 and 70 DF,  p-value: < 2.2e-16

### Correlation of External Indicators

The following Correlation factors were examined to see if there was any
impact on the total Etel Flower exports.

1.  Current Export Price Index - the correlation was 0.339713. Some
    correlation but not enough to impact the total Etel Flower Exports

2.  Birth - there is a negative correlation (-0.1504242), so if births
    decrease the export of Etel flowers decrease.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-41-1.png)<!-- -->

1.  Exports from Urbano - there is a slight correlation (0.3182532) but
    not enough to impact the total Etel Flower exports.

2.  Independence Day Presents Indicator - there is a small
    correlation (0.287213) but not enough to impact the total Etel
    Flower Exports.

3.  Temperature - there is a negative correlation between the average
    temperature in chulwalar and the exports of the Etel flower. In
    colder months exports increase and decrease in the warmer months.
    The correlation of Total Etel flower exports and temperatur
    is -0.453138.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-48-1.png)<!-- -->

1.  Satisfaction Index - there is only a slight correlation between the
    overall satisfaction index and the export of Etel Flowers. The
    correlation value was 0.2865672.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-50-1.png)<!-- -->

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-52-1.png)<!-- -->

1.  Yearly number of Globalisation Party members in Chulwalar - there is
    not a big enough correlation (0.2994635) to impact the exports of
    the Etel Flower.

2.  Monthly Average Export Price Index in chulwalar - there is not a big
    enough correlatin (0.3035506) to impact the exports of the
    Etel Flower. One thought is that continue growth has a postive
    affect on exports.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-55-1.png)<!-- -->

1.  Monthly Producer Price Index (PPI) for Etel in Chulwalar - there is
    not a big enough correlation (0.3374707) to impact the exports of
    the Etel Flower.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-57-1.png)<!-- -->

1.  National Holidays - there is a negative correlation (-0.01081446)
    between National Holidays and the exports of Etel flowers.
    Individuals may export more Etel flowers for National holidays then
    other days.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-59-1.png)<!-- -->

1.  The Total value of All companies in Chulwalar - there is not a big
    enough correlatin (0.3035506) to impact the exports of the
    Etel Flower.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-62-1.png)<!-- -->

1.  Month Inflation rate in Chulwalar - there is a negative
    correlation (-0.08378282) between inflation and the exports of the
    Etel flower. The negative correlation is seen with the export of the
    Red Etel flower (-0.0982151) but not the Blue Etel
    flower (0.02117817).

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-64-1.png)<!-- -->

1.  Monthly Producer Price Index for Etel in Chulwalar - - there is not
    a big enough correlatin (0.374707) to impact the exports of the
    Etel Flower.
    ![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-66-1.png)<!-- -->

2.  Influence National Holidays. This indicator looks at the months
    leading up to a National holiday to see if exports increase - there
    is a moderate correlation (0.4535836), but not sure this will help
    with forecasting future exports

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-69-1.png)<!-- -->

View correlation between exports and external indicators by offsetting the export data by one month.
----------------------------------------------------------------------------------------------------

The purpose of offsetting the export data by one month is to see if the
index change makes itself first noticeable on exports in the following
months.

External Satisfaction Index indicator is to be offset by one month, to
see if the index change makes itself first noticeable on exports in the
following months.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-72-1.png)<!-- -->

December 2013 was deleted from the data set to see what impact this
month has on the Etel Flower exports.

The satisfaction index indicator now has a negative correlation with the
Etel Flower Exports - -0.004445279 but this still isn't enough to have a
noticeable impact.

November and December 2013 were removed to see the overall impact on
exports of Etel Flowers. The impact is minimal with a correlation of
0.0446355.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-76-1.png)<!-- -->

November and December 2013 were removed from the Time Series data set to
see if it shows any impact to the overall export of the Etel flowers.
Again, there is a minimal impact with a correlation of 0.0446355.

The overall satisifcation and Government Party indicators also did not
have any impact on the overall exports of the Etel flowers.

Each of the external indicators were reviewed to see which ones should
be included in the final model.

The Correlation Coefficient Matrix shows that CEPI has a high
correlation with Overall Satisfication, Urbano Exports, Global Party
Members and Average Export Price Index. These will become the set of
indicators used later, although there is a risk of multicollinearity.

National Holidays, Urbano Exports, Global Party Members have a very low
correlation with one another. Therefore these will also become a set of
indicators used later.

Building Forecasting Model: using all external indicators with the Etel Flower Exports
--------------------------------------------------------------------------------------

Combining Chulwalar Export Price Index (CEPI), Satisfaction Index -
Government, Temperatur, Births, Overall Satisfaction Index, Urbano
Exports, Globalisation Party Members, Average Export Price Index,
National Holidays, Chulwalar Index, Inflation, and Independence Day
presents into one model did not produce any statistically signifcant
p-values for any of the external indicators. This indicates that having
all the external indicators in one model is not the best model to use
for forecasting.

Build Model with the Chulwaler Export Price Index indicator and the Etel Flower Exports
---------------------------------------------------------------------------------------

The Adjusted R Squared is at 0.866 which is good but the Chulwaler
Export Price Index does not appear to have a statistical impact on the
export of the Etel Flowers based on the p-values of the indicator.

Build Model with the Statisfaction Index to view its impact on the Etel Flower Exports
--------------------------------------------------------------------------------------

    # The Satisfaction Index (gov)  hardly changes the function of the model.
    ModelWithSIGov <- tslm(TotalEtelAsIs ~ trend + season + SIGov)
    summary(ModelWithSIGov)    

    ## 
    ## Call:
    ## tslm(formula = TotalEtelAsIs ~ trend + season + SIGov)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -345475 -110285   -8382  113926  461146 
    ## 
    ## Coefficients:
    ##             Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)  1303471      84010  15.516  < 2e-16 ***
    ## trend           9048       1103   8.203 2.80e-11 ***
    ## season2      -106455     101785  -1.046   0.3000    
    ## season3      -133300     101800  -1.309   0.1956    
    ## season4      -498901     101857  -4.898 8.12e-06 ***
    ## season5      -604908     101846  -5.939 1.71e-07 ***
    ## season6      -748213     101898  -7.343 7.78e-10 ***
    ## season7      -829933     102011  -8.136 3.63e-11 ***
    ## season8      -634890     102019  -6.223 5.82e-08 ***
    ## season9       592372     102083   5.803 2.87e-07 ***
    ## season10      197270     102194   1.930   0.0585 .  
    ## season11      224660     102328   2.195   0.0321 *  
    ## season12       -4578     102540  -0.045   0.9645    
    ## SIGov          -4901       2180  -2.248   0.0284 *  
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 176300 on 58 degrees of freedom
    ## Multiple R-squared:  0.8993, Adjusted R-squared:  0.8767 
    ## F-statistic: 39.85 on 13 and 58 DF,  p-value: < 2.2e-16

The Satisification Index - Government does seem to have statistical
significant impact on the Etel flower exports. The p-value is 0.0284 for
the Satisification Index - Government and the R-squared is 0.8767.

Build Model with the Temperature indicator and its impact on the Etel Flower Exports
------------------------------------------------------------------------------------

The temperature indicator does not do a good job impacting the overall
export of the Etel flowers. The Variance inflation factor is 9.40994 and
the p-value is 0.196136.

Build Model with National Holidays indicator to review its impact on the Etel flower exports
--------------------------------------------------------------------------------------------

National Holidays have some impact on the export of Etel Flowers. The
Adjusted R Squared is 0.8744 and the p-value 0.0534 for the National
Holiday indicator is somewhat statistically significant. The variance
inflation factor is high at 9.74823 but this indicator may still be used
in the final model.

Build Model with inflation indicator to review its impact on the Etel flower exports
------------------------------------------------------------------------------------

Inflation does not have a statistical impact on the exports of Etel
flowers as indicated by the p-value 0.563331 and the variance inflation
factor of 9.487. Therefore, the inflation indicator is not a good factor
to include in the final model.

Build Model with Independence Day Presents indicator to review its impact on the Etel flower exports
----------------------------------------------------------------------------------------------------

The buying of Independence Day presents does not have a statistical
impact on the exports of Etel flowers as indicated by the p-value
0.574184 and the variance inflation factor of 12.15354. Therefore, the
buying of Independence Day present indicator is not a good factor to
include in the final model.

Build Model with National Holiday indicator to review its impact on the Etel flower exports
-------------------------------------------------------------------------------------------

The Influence National Holiday indicator has more of an effect on the
Red Etel flower export than on the Blue Etel flower. The adjusted
Adjusted R Square is 0.8744 and the p-value for the indicator is 0.05336
which is mildly signifcant. The variation inflation factor for the total
Etel flower exports is 9.74823.

Building Models with High Correlating Indicators
================================================

High correlating indicators do not show a strong impact on the export of
Etel flowers. The adjusted R Square is 0.8706 but the p-values for each
of the indicators is not statistically significant.

Building Models with Low Correlating Indicators
===============================================

The low correlating indicators chosen were the National Holiday and the
Globalization of Party Members. Both seem to have an impact on the
exports of the Etel flowers. The adjusted R Square is 0.883 and both
p-values for the indicators are statistically significant (National
Holiday - 0.0457 and Globalization of Party Members - 0.0256). The
variance inflation factor is 10.64726 which is high and an indicator
this is not the best model.

Building Model with Trend and Season only and no other external indicators
==========================================================================

    ## 
    ## Call:
    ## tslm(formula = TotalEtelAsIs ~ trend + season)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -352676 -105634    5934  107814  481013 
    ## 
    ## Coefficients:
    ##             Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)  1370632      81168  16.886  < 2e-16 ***
    ## trend           8070       1048   7.702 1.75e-10 ***
    ## season2      -101964     105202  -0.969   0.3364    
    ## season3      -128812     105218  -1.224   0.2257    
    ## season4      -506178     105244  -4.810 1.08e-05 ***
    ## season5      -607122     105281  -5.767 3.14e-07 ***
    ## season6      -751654     105327  -7.136 1.59e-09 ***
    ## season7      -838360     105385  -7.955 6.51e-11 ***
    ## season8      -631474     105452  -5.988 1.35e-07 ***
    ## season9       592436     105531   5.614 5.60e-07 ***
    ## season10      202397     105619   1.916   0.0602 .  
    ## season11      232807     105718   2.202   0.0316 *  
    ## season12        8713     105827   0.082   0.9347    
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 182200 on 59 degrees of freedom
    ## Multiple R-squared:  0.8905, Adjusted R-squared:  0.8683 
    ## F-statistic:    40 on 12 and 59 DF,  p-value: < 2.2e-16

The seasonality and trend model is a fair model. The adjusted R Square
is 0.8683 and the p-values for some of the seasons are statistically
signifcant but not all. Mainly season 11.

Building Model without Trend and seasonality.
=============================================

This model does not work well. The adjusted R square is 0.0728 and none
of the p-values for the external indicators are of statisitical
significance.

    ## 
    ## Call:
    ## tslm(formula = TotalEtelAsIs ~ CEPI + SIExtern + UrbanoExports + 
    ##     GlobalisationPartyMembers + AEPI)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -826260 -397817   67869  307638 1276508 
    ## 
    ## Coefficients:
    ##                             Estimate Std. Error t value Pr(>|t|)
    ## (Intercept)               -9.702e+06  7.756e+06  -1.251    0.215
    ## CEPI                       1.948e+05  1.206e+05   1.616    0.111
    ## SIExtern                   1.287e+04  7.271e+04   0.177    0.860
    ## UrbanoExports              2.056e-01  5.904e-01   0.348    0.729
    ## GlobalisationPartyMembers -1.410e+01  2.531e+01  -0.557    0.579
    ## AEPI                      -8.937e+04  7.513e+04  -1.190    0.238
    ## 
    ## Residual standard error: 483400 on 66 degrees of freedom
    ## Multiple R-squared:  0.1381, Adjusted R-squared:  0.0728 
    ## F-statistic: 2.115 on 5 and 66 DF,  p-value: 0.07449

Etel Flower Export Model
========================

The model for the etel segment, including both subcategories, work best
with trend and seasonality. An attempt to improve the model by adding
Temperature showed no improvement worth mentioning. The adjusted R
Square for the total Etel flower exports is 0.863. Not all seasons for
the Red Etel flower are statistically significant but season 10 and 11
are. The Blue Etel flower does not show the same improvement.

Forecasting with Models with Shorten Time series
================================================

The time series data sets require that the time be shorten in order to
compare the produced forecasts with the current As Is data.

Check High Correlating Indicators
---------------------------------

The same results as seen in the previous models is present with this
model. The adjusted R Square is 0.8778 but none of the p-values for the
external indicators are statistically significant.

### Adding data to the 2013 indicator values in order to forecast

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-111-1.png)<!-- -->

There is a strong correlation between the As is data and the plan data
for 2013 for the Etel Flower Exports. The Linear regression comparison
supports the results with an adjusted R Square of 0.9144.

Check Low Correlating Indicators
--------------------------------

The adjusted R square is 0.8786 but none of the external indicators have
a p-value of statistical significance.

### Adding data to the 2013 Low correlating indicator values in order to forecast

The low correlating indicators forecast model follows the pattern of the
existing data for the Etel Flower exports. The linear regression
comparsion supports this forecasting model. The adjusted R square is
0.9144 and the F-statistic is 118.5,

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-116-1.png)<!-- -->

There is a strong correlation with the low correlating indicators and
the current as is data for 2013 and the plan data for 2013 for the Etel
Flower exports.

Forcasting with only Seasonality and Trend for the Etel Flower Exports
----------------------------------------------------------------------

The seasonality and trend work well with this forecasting model. The
adjust R Square is 0.8755 and again season 10 and 11 show statistical
significance.

### Adding data to the 2013 Seasonality and Trend for the Forecast model

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-119-1.png)<!-- -->

Trend and Seasonality continue to be the best model for the Etel Flower
exports. The forecasting model shows a pattern that follows even closer
to the current export pattern of the Etel flower. There is a strong
correlation between the current export Etel flower data and the plan
data for 2013. The linear regression supports this model. The adjusted R
Square is 0.9144 and the F-Statistic is 118.5

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-122-1.png)<!-- -->

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-123-1.png)<!-- -->

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-124-1.png)<!-- -->

Forecasting 2014 for the Etel Flower Exports with National Holidays and Globalisation Party Members
===================================================================================================

In looking at 2014 Forecasting of the Etel Flower exports, National
Holidays and Globalisation Party Member seem to have a positive impact
on the total exports of the Etel Flowers. The p-values are 0.04566 for
National Holidays indicator and 0.02557 for Globalisation Party Members
indicator both statistically significant.

    ## 
    ## Call:
    ## tslm(formula = TotalEtelAsIs ~ trend + season + NationalHolidays + 
    ##     GlobalisationPartyMembers)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -339086 -114138   16689  103127  426582 
    ## 
    ## Coefficients:
    ##                             Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)               2793808.47  625417.30   4.467 3.81e-05 ***
    ## trend                       17168.18    4089.10   4.199 9.53e-05 ***
    ## season2                   -111062.18   99222.63  -1.119  0.26770    
    ## season3                    -75389.44  105469.63  -0.715  0.47765    
    ## season4                   -390235.38  122037.29  -3.198  0.00226 ** 
    ## season5                   -643513.72  100478.56  -6.404 3.10e-08 ***
    ## season6                   -797144.07  101224.64  -7.875 1.11e-10 ***
    ## season7                   -892947.25  102129.12  -8.743 4.06e-12 ***
    ## season8                   -695159.60  103187.82  -6.737 8.72e-09 ***
    ## season9                    519652.89  104396.06   4.978 6.28e-06 ***
    ## season10                   120515.21  105748.72   1.140  0.25920    
    ## season11                   141827.86  107240.32   1.323  0.19128    
    ## season12                   123490.26  151355.81   0.816  0.41796    
    ## NationalHolidays          -214854.25  105152.08  -2.043  0.04566 *  
    ## GlobalisationPartyMembers     -31.35      13.67  -2.293  0.02557 *  
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 171700 on 57 degrees of freedom
    ## Multiple R-squared:  0.9061, Adjusted R-squared:  0.883 
    ## F-statistic: 39.28 on 14 and 57 DF,  p-value: < 2.2e-16

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-126-1.png)<!-- -->

Forecasting Exports for the Etel Flowers with Seasonality and Trend only for 2014
=================================================================================

Seasonality and Trend continue to show a good fit and work well with
forecasting for 2014. The adjusted R Square is 0.8683. With this
forecast model though Season 10 statistical significance is much lower
but Season 11 continues to show statistically signifcance in the Etel
flower exports for Chuluwala.

There continues to be a strong correlation between the current export
data and the plan data.

    ## 
    ## Call:
    ## tslm(formula = TotalEtelAsIs ~ trend + season)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -352676 -105634    5934  107814  481013 
    ## 
    ## Coefficients:
    ##             Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)  1370632      81168  16.886  < 2e-16 ***
    ## trend           8070       1048   7.702 1.75e-10 ***
    ## season2      -101964     105202  -0.969   0.3364    
    ## season3      -128812     105218  -1.224   0.2257    
    ## season4      -506178     105244  -4.810 1.08e-05 ***
    ## season5      -607122     105281  -5.767 3.14e-07 ***
    ## season6      -751654     105327  -7.136 1.59e-09 ***
    ## season7      -838360     105385  -7.955 6.51e-11 ***
    ## season8      -631474     105452  -5.988 1.35e-07 ***
    ## season9       592436     105531   5.614 5.60e-07 ***
    ## season10      202397     105619   1.916   0.0602 .  
    ## season11      232807     105718   2.202   0.0316 *  
    ## season12        8713     105827   0.082   0.9347    
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 182200 on 59 degrees of freedom
    ## Multiple R-squared:  0.8905, Adjusted R-squared:  0.8683 
    ## F-statistic:    40 on 12 and 59 DF,  p-value: < 2.2e-16

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-128-1.png)<!-- -->

Using other Modelling Approaches
================================

Exponential Smoothing
---------------------

The Exponential Smoothing does not seem to be the best model for
forecasting 2014. The predicted forecast shows flat exports for th Etel
Flower which is not indictive of past years.

    ## 
    ## Forecast method: Simple exponential smoothing
    ## 
    ## Model Information:
    ## Simple exponential smoothing 
    ## 
    ## Call:
    ##  ses(x = TotalEtelAsIs, h = 12) 
    ## 
    ##   Smoothing parameters:
    ##     alpha = 0.7395 
    ## 
    ##   Initial states:
    ##     l = 1195425.4826 
    ## 
    ##   sigma:  457693.8
    ## 
    ##      AIC     AICc      BIC 
    ## 2188.810 2188.984 2193.363 
    ## 
    ## Error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set 17461.77 457693.8 297227.3 -4.846428 21.14544 1.453283
    ##                    ACF1
    ## Training set 0.02266816
    ## 
    ## Forecasts:
    ##          Point Forecast     Lo 80   Hi 80      Lo 95   Hi 95
    ## Jan 2014        2125179 1538620.3 2711737 1228115.06 3022242
    ## Feb 2014        2125179 1395654.1 2854703 1009467.27 3240890
    ## Mar 2014        2125179 1276437.7 2973919  827141.42 3423216
    ## Apr 2014        2125179 1172017.3 3078340  667444.30 3582913
    ## May 2014        2125179 1077957.7 3172399  523592.49 3726765
    ## Jun 2014        2125179  991676.6 3258680  391636.90 3858720
    ## Jul 2014        2125179  911513.9 3338843  269038.63 3981318
    ## Aug 2014        2125179  836327.5 3414030  154050.92 4096306
    ## Sep 2014        2125179  765291.7 3485065   45411.04 4204946
    ## Oct 2014        2125179  697786.7 3552570  -57828.92 4308186
    ## Nov 2014        2125179  633333.1 3617024 -156402.12 4406759
    ## Dec 2014        2125179  571551.2 3678806 -250889.44 4501246

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-130-1.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-130-2.png)<!-- -->

Holt's linear trend method
--------------------------

The Holt's Linear Trend Method does not seem to be the best model for
forecasting 2014. The predicted forecast shows a relatively flat
forecast for exports for th Etel Flower which is not indictive of past
years.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-131-1.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-131-2.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-131-3.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-131-4.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-131-5.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-131-6.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-131-7.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-131-8.png)<!-- -->
![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-132-1.png)<!-- -->

Holt's auto seems to have the best forecast for the Etel flower exports
in 2014.

Holt-Winter's seasonal method
-----------------------------

The AIC is better than the regular Holts Method and the forecast for 201
Etel flower exports follow trends from past years exports.

    ## 
    ## Forecast method: Holt-Winters' additive method
    ## 
    ## Model Information:
    ## Holt-Winters' additive method 
    ## 
    ## Call:
    ##  hw(x = TotalEtelAsIs, h = 12, seasonal = "additive") 
    ## 
    ##   Smoothing parameters:
    ##     alpha = 0.1006 
    ##     beta  = 4e-04 
    ##     gamma = 1e-04 
    ## 
    ##   Initial states:
    ##     l = 1197857.198 
    ##     b = 10920.4281 
    ##     s=213227.6 432750.3 389222.1 773339.9 -385004.6 -600027.3
    ##            -533376.9 -405213.3 -324353.9 76198.07 175183 188055
    ## 
    ##   sigma:  172689.4
    ## 
    ##      AIC     AICc      BIC 
    ## 2076.452 2086.343 2112.879 
    ## 
    ## Error measures:
    ##                  ME     RMSE    MAE       MPE     MAPE      MASE
    ## Training set -19817 172689.4 137259 -3.310116 10.74612 0.6711232
    ##                    ACF1
    ## Training set -0.1543248
    ## 
    ## Forecasts:
    ##          Point Forecast   Lo 80   Hi 80     Lo 95   Hi 95
    ## Jan 2014        2008304 1786994 2229615 1669839.3 2346769
    ## Feb 2014        2005752 1783307 2228197 1665551.5 2345952
    ## Mar 2014        1917189 1693606 2140771 1575248.8 2259128
    ## Apr 2014        1527024 1302302 1751747 1183340.8 1870708
    ## May 2014        1456525 1230660 1682391 1111093.8 1801957
    ## Jun 2014        1338726 1111715 1565737  991542.2 1685909
    ## Jul 2014        1282438 1054279 1510598  933498.5 1631378
    ## Aug 2014        1507832 1278522 1737143 1157132.1 1858532
    ## Sep 2014        2676592 2446128 2907057 2324127.9 3029057
    ## Oct 2014        2302843 2071223 2534464 1948610.2 2657076
    ## Nov 2014        2356737 2123957 2589516 2000730.8 2712742
    ## Dec 2014        2147585 1913641 2381529 1789799.1 2505371

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-133-1.png)<!-- -->

    ## 
    ## Forecast method: Holt-Winters' multiplicative method
    ## 
    ## Model Information:
    ## Holt-Winters' multiplicative method 
    ## 
    ## Call:
    ##  hw(x = TotalEtelAsIs, h = 12, seasonal = "multiplicative") 
    ## 
    ##   Smoothing parameters:
    ##     alpha = 0.1007 
    ##     beta  = 0.0202 
    ##     gamma = 1e-04 
    ## 
    ##   Initial states:
    ##     l = 1185233.6784 
    ##     b = 11436.6691 
    ##     s=1.1484 1.3007 1.2775 1.5501 0.7138 0.5675
    ##            0.6356 0.7225 0.7983 1.0554 1.0793 1.1511
    ## 
    ##   sigma:  0.1215
    ## 
    ##      AIC     AICc      BIC 
    ## 2071.694 2081.585 2108.121 
    ## 
    ## Error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE      MASE
    ## Training set 2570.544 154506.4 126050.4 -1.274176 9.741218 0.6163191
    ##                    ACF1
    ## Training set -0.2582845
    ## 
    ## Forecasts:
    ##          Point Forecast     Lo 80   Hi 80     Lo 95   Hi 95
    ## Jan 2014        2134821 1802370.6 2467272 1626381.7 2643261
    ## Feb 2014        2018272 1701688.7 2334855 1534099.6 2502444
    ## Mar 2014        1990076 1674924.2 2305227 1508093.0 2472059
    ## Apr 2014        1517542 1274319.5 1760765 1145565.3 1889519
    ## May 2014        1384653 1159472.1 1609834 1040268.6 1729037
    ## Jun 2014        1228015 1024850.6 1431179  917301.9 1538728
    ## Jul 2014        1105178  918695.4 1291660  819977.4 1390378
    ## Aug 2014        1401176 1159448.3 1642903 1031485.6 1770866
    ## Sep 2014        3067063 2524835.0 3609292 2237796.7 3896330
    ## Oct 2014        2547465 2084968.1 3009962 1840136.8 3254794
    ## Nov 2014        2613831 2125584.2 3102077 1867122.3 3360539
    ## Dec 2014        2325692 1877988.5 2773396 1640988.6 3010396

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-133-2.png)<!-- -->

The additive model gives slightly better results than the multiplicative
model.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-134-1.png)<!-- -->

Innovations state space models for exponential smoothing
--------------------------------------------------------

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-137-1.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-137-2.png)<!-- -->

ARIMA Model
-----------

The data for the Etel Flower Export is stationary which is supported by
the Augmented Dickey-Fuller Test, but there is a warning indicating the
p-value is less than 0.01.

    ## Warning in adf.test(TotalEtelAsIs, alternative = "stationary"): p-value
    ## smaller than printed p-value

    ## 
    ##  Augmented Dickey-Fuller Test
    ## 
    ## data:  TotalEtelAsIs
    ## Dickey-Fuller = -5.5849, Lag order = 4, p-value = 0.01
    ## alternative hypothesis: stationary

The Kwiatkowki=Phillips-Schmidt-Shin Test supports that the p-value is
ate 0.1822 , which is statistically significant.

    ## 
    ##  KPSS Test for Level Stationarity
    ## 
    ## data:  TotalEtelAsIs
    ## KPSS Level = 0.64854, Truncation lag parameter = 1, p-value =
    ## 0.01822

The data is differenced and retested

    ## Warning in adf.test(ChulwalarDiff, alternative = "stationary"): p-value
    ## smaller than printed p-value

    ## 
    ##  Augmented Dickey-Fuller Test
    ## 
    ## data:  ChulwalarDiff
    ## Dickey-Fuller = -5.531, Lag order = 4, p-value = 0.01
    ## alternative hypothesis: stationary

    ## Warning in kpss.test(ChulwalarDiff): p-value greater than printed p-value

    ## 
    ##  KPSS Test for Level Stationarity
    ## 
    ## data:  ChulwalarDiff
    ## KPSS Level = 0.021036, Truncation lag parameter = 1, p-value = 0.1

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-141-1.png)<!-- -->

The following test method is used to distinguish the number of "normal"
differencing rounds and seasonal differencing rounds. Seasonal
differencing is used for data that is dominated by seasonality which
Etel Flower exports seem to be. A lag as been added to the time series
data for the Etel Flower data.

    ## [1] 0

    ## [1] 1

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2009  303548  354063   53281   50375   46292  214397  137476   36309
    ## 2010   54248  268773  128759 -327631  278541  281148 -358866  169492
    ## 2011  -42197 -202633  -79832  221181 -245848 -320721  250808  210270
    ## 2012  -75519  339369  137552  -26628  339430  120855  143853   12334
    ## 2013  589749  -74700   26664  737070 -252534  114043   57237  -80471
    ##          Sep     Oct     Nov     Dec
    ## 2009  266298 -147817  339548   13767
    ## 2010  353925  208330 -179713   83972
    ## 2011  -32217 -264680  282552   14928
    ## 2012   27063  586311  345649  -95844
    ## 2013  670595  127710  -21652  444013

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-142-1.png)<!-- -->

    ## 
    ##  Augmented Dickey-Fuller Test
    ## 
    ## data:  ChulwalarDiff_lag
    ## Dickey-Fuller = -3.3973, Lag order = 3, p-value = 0.0648
    ## alternative hypothesis: stationary

    ## Warning in kpss.test(ChulwalarDiff_lag): p-value greater than printed p-
    ## value

    ## 
    ##  KPSS Test for Level Stationarity
    ## 
    ## data:  ChulwalarDiff_lag
    ## KPSS Level = 0.26915, Truncation lag parameter = 1, p-value = 0.1

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-142-2.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-142-3.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-142-4.png)<!-- -->

ARIMA modelling
---------------

    ## Series: TotalEtelAsIs 
    ## ARIMA(0,1,0)                    
    ## 
    ## sigma^2 estimated as 2.24e+11:  log likelihood=-1028.53
    ## AIC=2059.07   AICc=2059.13   BIC=2061.33
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE    MASE
    ## Training set 10885.72 469992.2 316754.4 -4.183168 22.00733 1.54876
    ##                    ACF1
    ## Training set -0.2078636

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-1.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(1,1,0)                    
    ## 
    ## Coefficients:
    ##           ar1
    ##       -0.2054
    ## s.e.   0.1156
    ## 
    ## sigma^2 estimated as 2.174e+11:  log likelihood=-1026.99
    ## AIC=2057.98   AICc=2058.16   BIC=2062.51
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set 13820.52 459745.2 299334.9 -4.672899 21.17425 1.463588
    ##                     ACF1
    ## Training set -0.02108637

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-2.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(1,1,1)                    
    ## 
    ## Coefficients:
    ##          ar1      ma1
    ##       0.5356  -0.9577
    ## s.e.  0.1113   0.0430
    ## 
    ## sigma^2 estimated as 1.836e+11:  log likelihood=-1021.16
    ## AIC=2048.32   AICc=2048.68   BIC=2055.11
    ## 
    ## Training set error measures:
    ##                    ME   RMSE    MAE       MPE     MAPE     MASE
    ## Training set 60565.25 419506 278583 -3.430148 20.34803 1.362122
    ##                      ACF1
    ## Training set -0.007510009

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-3.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(2,1,1)                    
    ## 
    ## Coefficients:
    ##          ar1      ar2      ma1
    ##       0.5514  -0.0368  -0.9554
    ## s.e.  0.1228   0.1214   0.0433
    ## 
    ## sigma^2 estimated as 1.86e+11:  log likelihood=-1021.11
    ## AIC=2050.23   AICc=2050.84   BIC=2059.28
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set 61421.92 419159.8 282807.5 -3.386659 20.62324 1.382777
    ##                     ACF1
    ## Training set -0.03269786

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-4.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(2,1,2)                    
    ## 
    ## Coefficients:
    ##           ar1     ar2     ma1      ma2
    ##       -0.4041  0.5955  0.0333  -0.9520
    ## s.e.   0.1098  0.1098  0.0521   0.0512
    ## 
    ## sigma^2 estimated as 1.724e+11:  log likelihood=-1018.67
    ## AIC=2047.34   AICc=2048.27   BIC=2058.66
    ## 
    ## Training set error measures:
    ##                   ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set 55996.3 400535.6 272287.9 -3.192989 20.05191 1.331342
    ##                    ACF1
    ## Training set 0.05235937

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-5.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(3,1,2)                    
    ## 
    ## Coefficients:
    ##           ar1     ar2      ar3     ma1      ma2
    ##       -0.3406  0.5094  -0.1498  0.0444  -0.9439
    ## s.e.   0.1218  0.1221   0.1202  0.0474   0.0470
    ## 
    ## sigma^2 estimated as 1.701e+11:  log likelihood=-1017.91
    ## AIC=2047.81   AICc=2049.12   BIC=2061.39
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set 60035.76 394839.8 283670.3 -2.931351 20.86698 1.386996
    ##                     ACF1
    ## Training set -0.03143675

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-6.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(3,1,3)                    
    ## 
    ## Coefficients:
    ##           ar1      ar2     ar3      ma1     ma2      ma3
    ##       -0.2758  -0.4063  0.5282  -0.1579  0.2256  -0.9625
    ## s.e.   0.1394   0.1100  0.1275   0.0978  0.1038   0.0853
    ## 
    ## sigma^2 estimated as 1.738e+11:  log likelihood=-1018.64
    ## AIC=2051.27   AICc=2053.05   BIC=2067.11
    ## 
    ## Training set error measures:
    ##                   ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set 56221.9 396058.6 263240.5 -2.968433 18.88281 1.287105
    ##                    ACF1
    ## Training set 0.05685117

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-7.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(3,1,1)                    
    ## 
    ## Coefficients:
    ##          ar1     ar2      ar3      ma1
    ##       0.5332  0.0387  -0.1576  -0.9451
    ## s.e.  0.1207  0.1322   0.1192   0.0431
    ## 
    ## sigma^2 estimated as 1.839e+11:  log likelihood=-1020.26
    ## AIC=2050.53   AICc=2051.45   BIC=2061.84
    ## 
    ## Training set error measures:
    ##                    ME   RMSE      MAE       MPE     MAPE     MASE
    ## Training set 65859.38 413668 287169.7 -3.017836 20.98778 1.404106
    ##                     ACF1
    ## Training set -0.06767524

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-8.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(3,1,2)                    
    ## 
    ## Coefficients:
    ##           ar1     ar2      ar3     ma1      ma2
    ##       -0.3406  0.5094  -0.1498  0.0444  -0.9439
    ## s.e.   0.1218  0.1221   0.1202  0.0474   0.0470
    ## 
    ## sigma^2 estimated as 1.701e+11:  log likelihood=-1017.91
    ## AIC=2047.81   AICc=2049.12   BIC=2061.39
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set 60035.76 394839.8 283670.3 -2.931351 20.86698 1.386996
    ##                     ACF1
    ## Training set -0.03143675

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-9.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(1,1,3)                    
    ## 
    ## Coefficients:
    ##          ar1      ma1     ma2      ma3
    ##       0.3980  -0.8255  0.0031  -0.1227
    ## s.e.  0.2521   0.2524  0.2183   0.1489
    ## 
    ## sigma^2 estimated as 1.872e+11:  log likelihood=-1020.82
    ## AIC=2051.64   AICc=2052.56   BIC=2062.95
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set 61338.98 417381.6 279203.2 -3.304679 20.40418 1.365154
    ##                     ACF1
    ## Training set -0.01613915

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-10.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(2,1,3)                    
    ## 
    ## Coefficients:
    ##           ar1      ar2     ma1      ma2      ma3
    ##       -1.1884  -0.1895  1.0274  -0.8487  -0.8956
    ## s.e.   0.1536   0.1535  0.2043   0.0964   0.1831
    ## 
    ## sigma^2 estimated as 1.56e+11:  log likelihood=-1016.68
    ## AIC=2045.36   AICc=2046.67   BIC=2058.94
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set 59423.55 378168.1 294500.1 -2.845444 21.91275 1.439948
    ##                    ACF1
    ## Training set 0.01497287

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-11.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(2,2,3)                    
    ## 
    ## Coefficients:
    ##           ar1     ar2      ma1      ma2     ma3
    ##       -0.4189  0.5809  -1.0014  -0.9851  0.9946
    ## s.e.   0.1062  0.1062   0.0664   0.0503  0.0661
    ## 
    ## sigma^2 estimated as 1.685e+11:  log likelihood=-1007.22
    ## AIC=2026.44   AICc=2027.78   BIC=2039.93
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE    MASE
    ## Training set 13591.95 389968.3 271275.1 -5.646689 20.46811 1.32639
    ##                    ACF1
    ## Training set 0.07307373

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-12.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(2,3,2)                    
    ## 
    ## Coefficients:
    ##           ar1      ar2      ma1     ma2
    ##       -0.1902  -0.0549  -1.9947  1.0000
    ## s.e.   0.1217   0.1208   0.0558  0.0555
    ## 
    ## sigma^2 estimated as 2.356e+11:  log likelihood=-1005.86
    ## AIC=2021.72   AICc=2022.67   BIC=2032.89
    ## 
    ## Training set error measures:
    ##                     ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set -9029.484 461153.8 309811.9 -4.878339 21.42473 1.514814
    ##                     ACF1
    ## Training set -0.01924413

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-143-13.png)<!-- -->

Based on the LFung-Box test below the data is not independently
distributed because the p-value is 2.19 which gives enough evidence to
reject the null hypothesis that the data is independently distributed.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-144-1.png)<!-- -->

    ## 
    ##  Box-Ljung test
    ## 
    ## data:  residuals(Model_ARIMA_12)
    ## X-squared = 46.18, df = 8, p-value = 2.197e-07

Seasonal ARIMA modelling
------------------------

The more the seasonal aspect is changed, the better the results based on
AIC, AICc and BIC. Theoretically the models should more and more
suitable for the forecast. However, a look at the plot of the forecasts
shows that the changes are making the data less and less convincing and
thus unuseable.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-145-1.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(0,0,0)(1,0,0)[12] with non-zero mean 
    ## 
    ## Coefficients:
    ##         sar1  intercept
    ##       0.8791  1476037.4
    ## s.e.  0.0444   135244.5
    ## 
    ## sigma^2 estimated as 6.777e+10:  log likelihood=-1007.86
    ## AIC=2021.72   AICc=2022.07   BIC=2028.55
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE        MPE     MAPE    MASE
    ## Training set 62343.65 256689.5 194587.8 0.05466362 14.82089 0.95143
    ##                    ACF1
    ## Training set 0.07066295

    ## Series: TotalEtelAsIs 
    ## ARIMA(0,1,1)(0,1,1)[12]                    
    ## 
    ## Coefficients:
    ##           ma1     sma1
    ##       -0.9102  -0.6446
    ## s.e.   0.0678   0.2063
    ## 
    ## sigma^2 estimated as 4.546e+10:  log likelihood=-810.93
    ## AIC=1627.85   AICc=1628.29   BIC=1634.08
    ## 
    ## Training set error measures:
    ##                     ME     RMSE      MAE       MPE     MAPE      MASE
    ## Training set -3607.306 189704.1 135489.8 -2.864112 10.12317 0.6624726
    ##                    ACF1
    ## Training set -0.1808033

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-145-2.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-145-3.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(2,3,2)(1,1,1)[12]                    
    ## 
    ## Coefficients:
    ##           ar1      ar2      ma1     ma2     sar1     sma1
    ##       -0.8074  -0.6593  -1.9804  0.9974  -0.3563  -0.1610
    ## s.e.   0.0982   0.1000   0.0734  0.0725   0.2816   0.3205
    ## 
    ## sigma^2 estimated as 4.929e+10:  log likelihood=-789.61
    ## AIC=1593.23   AICc=1595.51   BIC=1607.53
    ## 
    ## Training set error measures:
    ##                     ME     RMSE      MAE       MPE     MAPE      MASE
    ## Training set -17124.16 186845.5 129418.7 -2.576346 9.671933 0.6327881
    ##                     ACF1
    ## Training set -0.07718252

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-145-4.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-145-5.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(1,0,1)(1,1,1)[12] with drift         
    ## 
    ## Coefficients:
    ##          ar1      ma1    sar1     sma1     drift
    ##       0.0529  -0.2166  0.1426  -0.7595  8211.122
    ## s.e.  0.3959   0.3731  0.3241   0.4232  1057.928
    ## 
    ## sigma^2 estimated as 4.355e+10:  log likelihood=-821.18
    ## AIC=1654.36   AICc=1655.94   BIC=1666.92
    ## 
    ## Training set error measures:
    ##                     ME     RMSE      MAE       MPE     MAPE      MASE
    ## Training set -1960.418 182403.2 133660.4 -2.755316 9.997192 0.6535278
    ##                      ACF1
    ## Training set -0.003556865

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-145-6.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-145-7.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(2,3,2)(1,4,2)[12]                    
    ## 
    ## Coefficients:

    ## Warning in sqrt(diag(x$var.coef)): NaNs produced

    ##           ar1      ar2      ma1     ma2    sar1     sma1    sma2
    ##       -0.9573  -0.9985  -1.1358  0.1358  -0.731  -0.5097  0.0399
    ## s.e.   0.0638   0.0016   0.4299  0.4713     NaN      NaN     NaN
    ## 
    ## sigma^2 estimated as 1.526e+12:  log likelihood=-353.25
    ## AIC=722.5   AICc=734.5   BIC=730.86
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE     MASE
    ## Training set 13377.73 544801.2 234374.8 0.9640717 15.00136 1.145967
    ##                    ACF1
    ## Training set -0.3006175

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-145-8.png)<!-- -->

Auto-ARIMA modelling
--------------------

    ## Series: TotalEtelAsIs 
    ## ARIMA(3,0,2)(1,1,0)[12] with drift         
    ## 
    ## Coefficients:
    ##          ar1     ar2     ar3      ma1      ma2     sar1     drift
    ##       0.0371  0.2713  0.5030  -0.0998  -0.4695  -0.4017  9852.810
    ## s.e.  0.1780  0.1780  0.1157   0.2018   0.1828   0.1379  3240.753
    ## 
    ## sigma^2 estimated as 3.911e+10:  log likelihood=-814.54
    ## AIC=1645.08   AICc=1647.91   BIC=1661.84
    ## 
    ## Training set error measures:
    ##                     ME     RMSE      MAE       MPE     MAPE      MASE
    ## Training set -1264.393 169669.5 128332.6 -2.233268 9.440145 0.6274777
    ##                      ACF1
    ## Training set -0.001515626

    ##           CV          AIC         AICc          BIC        AdjR2 
    ## 4.081446e+10 1.757920e+03 1.765288e+03 1.789793e+03 8.682746e-01

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-146-1.png)<!-- -->

    ## 
    ##  Box-Ljung test
    ## 
    ## data:  residuals(Model_auto.arima)
    ## X-squared = 8.5341, df = 8, p-value = 0.3831

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-146-2.png)<!-- -->

    ##          Point Forecast     Lo 80   Hi 80     Lo 95   Hi 95
    ## Jan 2014        2068608 1815172.2 2322044 1681011.3 2456205
    ## Feb 2014        1948186 1694252.2 2202120 1559827.8 2336544
    ## Mar 2014        1918326 1659356.5 2177295 1522266.5 2314385
    ## Apr 2014        1638644 1352676.7 1924611 1201294.9 2075992
    ## May 2014        1349768 1063278.7 1636256  911620.6 1787914
    ## Jun 2014        1247277  960709.7 1533844  809010.2 1685544
    ## Jul 2014        1172341  880242.3 1464439  725614.7 1619067
    ## Aug 2014        1395261 1103123.0 1687398  948474.8 1842046
    ## Sep 2014        2942839 2650114.0 3235565 2495154.6 3390524
    ## Oct 2014        2446561 2152513.4 2740608 1996854.2 2896267
    ## Nov 2014        2493834 2199763.9 2787904 2044092.7 2943575
    ## Dec 2014        2080932 1786370.3 2375494 1630438.6 2531426

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2014 2068608 1948186 1918326 1638644 1349768 1247277 1172341 1395261
    ##          Sep     Oct     Nov     Dec
    ## 2014 2942839 2446561 2493834 2080932

Dynamic regression models
-------------------------

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-147-1.png)<!-- -->

    ## Series: TotalEtelAsIs 
    ## ARIMA(2,2,0)                    
    ## 
    ## Coefficients:
    ##           ar1      ar2  CEPI_lagged
    ##       -0.7910  -0.4090    -189524.6
    ## s.e.   0.1183   0.1198     212476.4
    ## 
    ## sigma^2 estimated as 2.959e+11:  log likelihood=-856.23
    ## AIC=1720.46   AICc=1721.08   BIC=1729.46
    ## 
    ## Training set error measures:
    ##                     ME   RMSE    MAE       MPE     MAPE     MASE
    ## Training set -5548.795 574848 416947 -2.292006 27.37392 2.038648
    ##                     ACF1
    ## Training set -0.08476448

    ## Series: TotalEtelAsIs 
    ## ARIMA(2,1,0)(1,1,0)[12]                    
    ## 
    ## Coefficients:
    ##           ar1      ar2     sar1  CEPI_lagged
    ##       -0.8380  -0.6707  -0.5724     67894.04
    ## s.e.   0.1043   0.1070   0.1332     76622.88
    ## 
    ## sigma^2 estimated as 3.476e+10:  log likelihood=-643.79
    ## AIC=1297.58   AICc=1298.71   BIC=1307.97
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE      MASE
    ## Training set 2464.261 178508.3 127632.1 -1.259806 9.067804 0.6240525
    ##                     ACF1
    ## Training set -0.02199872

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-147-2.png)<!-- -->![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-147-3.png)<!-- -->

    ## 
    ##  Box-Ljung test
    ## 
    ## data:  residuals(Model_dynreg_auto.arima)
    ## X-squared = 15.574, df = 8, p-value = 0.0489

    ## Series: TotalEtelAsIs 
    ## ARIMA(2,1,0)(1,1,0)[12]                    
    ## 
    ## Coefficients:
    ##           ar1      ar2     sar1  CEPI_lagged
    ##       -0.8380  -0.6707  -0.5724     67894.04
    ## s.e.   0.1043   0.1070   0.1332     76622.88
    ## 
    ## sigma^2 estimated as 3.476e+10:  log likelihood=-643.79
    ## AIC=1297.58   AICc=1298.71   BIC=1307.97
    ## 
    ## Training set error measures:
    ##                    ME     RMSE      MAE       MPE     MAPE      MASE
    ## Training set 2464.261 178508.3 127632.1 -1.259806 9.067804 0.6240525
    ##                     ACF1
    ## Training set -0.02199872

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-147-4.png)<!-- -->

    ##          Point Forecast     Lo 80   Hi 80     Lo 95   Hi 95
    ## Jan 2014        2142641 1903700.8 2381581 1777213.6 2508068
    ## Feb 2014        1996013 1753958.4 2238068 1625822.3 2366204
    ## Mar 2014        1951716 1705284.7 2198148 1574831.7 2328601
    ## Apr 2014        1625985 1324182.5 1927787 1164417.9 2087552
    ## May 2014        1432031 1123941.4 1740120  960848.9 1903212
    ## Jun 2014        1315721  999737.7 1631703  832466.4 1798975
    ## Jul 2014        1308007  962967.4 1653047  780314.4 1835700
    ## Aug 2014        1478998 1125747.1 1832250  938747.2 2019250
    ## Sep 2014        2923917 2561154.2 3286680 2369119.0 3478715
    ## Oct 2014        2522277 2140496.5 2904057 1938394.2 3106159
    ## Nov 2014        2566337 2175452.6 2957221 1968531.0 3164143
    ## Dec 2014        2109905 1709051.5 2510759 1496852.4 2722958

    ##          Jan     Feb     Mar     Apr     May     Jun     Jul     Aug
    ## 2014 2142641 1996013 1951716 1625985 1432031 1315721 1308007 1478998
    ##          Sep     Oct     Nov     Dec
    ## 2014 2923917 2522277 2566337 2109905

New Model
=========

As trend and seasonality have been shown to forecast well on their own,
we will add the new combination to trend and seasonality in order to try
to improve the forecast. Inflation and NationalHolidays additional
Seasonality and Trend only.

    ## 
    ## Call:
    ## tslm(formula = TotalEtelAsIs ~ trend + season + Inflation + NationalHolidays)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -326416 -114404    3978  112658  473492 
    ## 
    ## Coefficients:
    ##                  Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)       1427775      88398  16.152  < 2e-16 ***
    ## trend                8104       1015   7.987 7.22e-11 ***
    ## season2           -101062     101852  -0.992   0.3253    
    ## season3            -57716     108042  -0.534   0.5953    
    ## season4           -372675     124961  -2.982   0.0042 ** 
    ## season5           -608371     101929  -5.969 1.62e-07 ***
    ## season6           -752352     101972  -7.378 7.46e-10 ***
    ## season7           -839325     102029  -8.226 2.90e-11 ***
    ## season8           -631888     102092  -6.189 7.03e-08 ***
    ## season9            590700     102175   5.781 3.27e-07 ***
    ## season10           198226     102296   1.938   0.0576 .  
    ## season11           226670     102441   2.213   0.0309 *  
    ## season12           206842     149352   1.385   0.1715    
    ## Inflation          -35130      24890  -1.411   0.1636    
    ## NationalHolidays  -205764     108214  -1.901   0.0623 .  
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 176400 on 57 degrees of freedom
    ## Multiple R-squared:  0.9009, Adjusted R-squared:  0.8765 
    ## F-statistic:    37 on 14 and 57 DF,  p-value: < 2.2e-16

    ## 
    ## Call:
    ## tslm(formula = TotalEtelAsIs ~ trend + season)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -352676 -105634    5934  107814  481013 
    ## 
    ## Coefficients:
    ##             Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)  1370632      81168  16.886  < 2e-16 ***
    ## trend           8070       1048   7.702 1.75e-10 ***
    ## season2      -101964     105202  -0.969   0.3364    
    ## season3      -128812     105218  -1.224   0.2257    
    ## season4      -506178     105244  -4.810 1.08e-05 ***
    ## season5      -607122     105281  -5.767 3.14e-07 ***
    ## season6      -751654     105327  -7.136 1.59e-09 ***
    ## season7      -838360     105385  -7.955 6.51e-11 ***
    ## season8      -631474     105452  -5.988 1.35e-07 ***
    ## season9       592436     105531   5.614 5.60e-07 ***
    ## season10      202397     105619   1.916   0.0602 .  
    ## season11      232807     105718   2.202   0.0316 *  
    ## season12        8713     105827   0.082   0.9347    
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 182200 on 59 degrees of freedom
    ## Multiple R-squared:  0.8905, Adjusted R-squared:  0.8683 
    ## F-statistic:    40 on 12 and 59 DF,  p-value: < 2.2e-16

The adjusted R square for the Inflation and National Holiday model is
0.8765 whereas the adjusted R Square for the Seasonality and Trend model
is 0.8683. The Inflation and National Holiday model seems to work a
little better but inflation is not statistically signifcant with a
p-value of 0.1636.

Forecasting with the New Model
------------------------------

There is a very strong correlation between the new model and the forcast
plan using the Inflation and National Holiday indicators.

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-150-1.png)<!-- -->

    ##          Point Forecast     Lo 80   Hi 80     Lo 95   Hi 95
    ## Jan 2013        1760202 1525178.1 1995226 1396258.6 2124146
    ## Feb 2013        1726107 1490947.7 1961266 1361954.2 2090260
    ## Mar 2013        1643963 1373595.2 1914332 1225288.3 2062639
    ## Apr 2013        1354102 1084589.1 1623615  936751.3 1771453
    ## May 2013        1287073 1051975.2 1522170  923015.5 1651130
    ## Jun 2013        1111051  876065.7 1346036  747167.6 1474934
    ## Jul 2013        1023601  788559.0 1258643  659629.9 1387572
    ## Aug 2013        1265108 1029964.5 1500251  900979.8 1629236
    ## Sep 2013        2376393 2141153.4 2611632 2012116.0 2740669
    ## Oct 2013        2061241 1825757.2 2296725 1696585.6 2425897
    ## Nov 2013        2106321 1871135.3 2341507 1742127.2 2470516
    ## Dec 2013        1887107 1652073.0 2122142 1523148.0 2251067

Trend and Seasonality only as benchmark
---------------------------------------

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-153-1.png)<!-- -->

    ##          Point Forecast     Lo 80   Hi 80     Lo 95   Hi 95
    ## Jan 2013        1755615 1519741.4 1991488 1390553.3 2120676
    ## Feb 2013        1717202 1481328.6 1953076 1352140.5 2082264
    ## Mar 2013        1715520 1479646.6 1951394 1350458.5 2080582
    ## Apr 2013        1250135 1014262.0 1486009  885073.9 1615197
    ## May 2013        1279815 1043941.8 1515689  914753.7 1644877
    ## Jun 2013        1113110  877236.8 1348984  748048.7 1478172
    ## Jul 2013        1028955  793081.8 1264829  663893.7 1394017
    ## Aug 2013        1256600 1020727.0 1492474  891538.9 1621662
    ## Sep 2013        2365726 2129853.0 2601600 2000664.9 2730788
    ## Oct 2013        2046428 1810554.4 2282301 1681366.3 2411489
    ## Nov 2013        2096791 1860918.0 2332665 1731729.9 2461853
    ## Dec 2013        1882065 1646192.0 2117939 1517003.9 2247127

Forecasting 2014 with New Model
-------------------------------

![](KClark_ChulwalarCaseStudy_Unit10_files/figure-markdown_strict/unnamed-chunk-156-1.png)<!-- -->

Comparison of Models
====================

When reviewing the correlation between the forecasting models -
Model\_dynreg\_auto.arima\_PointForecast Model has the highest
correlation at 0.9534608.

Based on the percentual differences the Trend and Seasonality model
works best to forecast for the Etel exports in 2014.

Final Summary
=============

Even though some external indicators provided a high correlation and
adjusted R square they did not provide a statistical impact on the Etel
flower exports based on the examination of the p-value. The Etel Flower
exports seem to be most impacted by trend and seasonality of the growing
season of the flowers, therefore the best models were those that only
looked at trend and seasonality. The Holt - Winter's family models
performed well.
