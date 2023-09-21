p8105_hw1_nl2835
================
Nancy Le
09-21-2023

I’m an R Markdown document!

``` r
library(moderndive)
data("early_january_weather")
```

The “early_january_weather dataset describes hourly meteorological data
for LGA, JFK, and EWR for the month of January 2013. This is a subset of
the weather data frame from nycflights13.

The format of this dataset is a dataframe of `358` rows and `15` columns
representing hourly measurements and 15 variables. Some important
variables are origin (meaning the weather station), year, month, day,
hour, temp, and dewp.

``` r
mean_temp <- mean(early_january_weather$temp)
```

The mean temperature is `39.5821229`.

``` r
library(ggplot2)

ggplot(data = early_january_weather, aes(x = hour, y = temp, color = humid)) + geom_point()
```

![](template--1-_files/figure-gfm/yx_scatter-1.png)<!-- -->

    ## Saving 7 x 5 in image
