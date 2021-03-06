Life Expectancy at Birth
========================================================


Developing Data Products

Guisb


Data Product
========================================================

Life expectancy at birth indicates the number of years a newborn infant would live if prevailing patterns of mortality at the time of its birth were to stay the same throughout its life.

This application permits forecasting Life Expectancy at Birth for the ten countries best classified by the World Bank, using the size of its Gross Domestic Product.

Computes univariate time series models estimated country by country using ARIMA models, Smoothing (ETS) and Decomposition, throught the Forecast package.



Data Source
========================================================

This data product Uses as data source the indicator Life expectancy at birth (SP.DYN.LE00.IN) of World Bank, in the period from 1980 to 2013. 

The datasets were obtained from the World Bank, using the WDI package.


The indicator used
========================================================

The indicator, from World Bank, used is derived from male and female life expectancy at birth from other sources such as: (1) United Nations Population Division. World Population Prospects, (2) United Nations Statistical Division. Population and Vital Statistics Report (various years), (3) Census reports and other statistical publications from national statistical offices, (4) Eurostat: Demographic Statistics, (5) Secretariat of the Pacific Community: Statistics and Demography Programme, and (6) U.S. Census Bureau: International Database.



Code executed inside this presentation
========================================================




```r
fit_arima <- auto.arima(dataforecast)
plot(forecast(fit_arima, h=10),  plot.conf=TRUE, col="#166BE2", fcol=4)
```

![plot of chunk unnamed-chunk-2](dataproducts-figure/unnamed-chunk-2-1.png) 
