# Case-Study-10
Karen Clark
MSDS 6306 DOING DATA SCIENCE - 404

The purpose of this case study is to provide Chulwalar, part of the Urbano islands.  The main exports are flowers that are known for their winter blooming; Efak, Wuge, and the Etel flower.  This forecast study looks at the Etel flower only.   Chulwalar officials want to know if external factors impact the exports of the Etel flower.  For example, Independence Day is celebrated on December 1st - does the need to buy Independence day presents increase producers exports of the Etel flower.  

The data is divided into three different sets:

1. Etel As Is - current export data
2. Etel Plan Data - what do future exports of the Etel flower look like
3. External Indicators

Data sets were transformed into time series data for data analysis.  Several different methods were examine to evaluate which model worked best to forecast 2014 exports for the Etel flower.

1.  Exponential smoothing
2.  Simple expontential smoothing
3.  Holt's linear trend method                                            
4.  Holt-Winter's seasonal method
5.  Innovations state space models for exponential smoothing
6.  ARIMA
7.  ARIMA modelling
8.  Seasonal ARIMA modelling
9.  Auto-ARIMA modelling           
10.  Dynamic regression models  

The models were examined using all the external indicators that were identified to have a high correlation and then indicators that had low correlation between each other.

1.  Monthly Change in Export Price Index (CEPI)
2.  Monthly Satisfaction Index (SI) government based data
3.  Average monthly temperatures in Chulwalar
4.  Monthly births in Chulwalar
5.  Monthly Satisfaction Index (SI) external index 
6.  Yearly Exports from Urbano
7.  Yearly number of Globalisation Party members in Chulwalar
8.  Monthly Average Export Price Index for Chulwalar
9.  Monthly Producer Price Index (PPI) for Etel in Chulwalar
10. National Holidays
11. Chulwalar Index (Total value of all companies in Chulwalar)
12. Monthly Inflation rate in Chulwalar
13. Proposed spending for National Holidays
14. Influence of National Holiday


Even though some external indicators provided a high correlation and adjusted R square they did not provide a statistical impact on the Etel flower exports based on the examination of the p-value.  The Etel Flower exports seem to be most impacted by trend and seasonality of the growing season of the flowers, therefore the best models were those that only looked at trend and seasonality.  The Holt - Winter's family models performed well.



















R Session Info:

R version 3.3.0 (2016-05-03)
Platform: x86_64-w64-mingw32/x64 (64-bit)
Running under: Windows >= 8 x64 (build 9200)

locale:
[1] LC_COLLATE=English_United States.1252  LC_CTYPE=English_United States.1252    LC_MONETARY=English_United States.1252
[4] LC_NUMERIC=C                           LC_TIME=English_United States.1252    

attached base packages:
[1] tcltk     stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
[1] fmsb_0.5.2        fpp_0.5           lmtest_0.9-34     expsmooth_2.3     fma_2.2           tseries_0.10-35  
[7] forecast_7.1      timeDate_3012.100 zoo_1.7-13       

loaded via a namespace (and not attached):
 [1] Rcpp_0.12.5      magrittr_1.5     munsell_0.4.3    colorspace_1.2-6 lattice_0.20-33  R6_2.1.2        
 [7] quadprog_1.5-5   plyr_1.8.3       stringr_1.0.0    httr_1.1.0       tools_3.3.0      nnet_7.3-12     
[13] parallel_3.3.0   grid_3.3.0       gtable_0.2.0     yaml_2.1.13      digest_0.6.9     crayon_1.3.1    
[19] ggplot2_2.1.0    bitops_1.0-6     RCurl_1.95-4.8   testthat_1.0.2   memoise_1.0.0    fracdiff_1.4-2  
[25] stringi_1.0-1    scales_0.4.0     swirl_2.4.1  
