bridges\_HW
================
David Young
2/2/2021

    ## Warning: package 'data.table' was built under R version 3.6.3

    ## Warning: package 'readr' was built under R version 3.6.3

``` r
bridges = fread('WI10.txt')
new.bridges = data.frame(bridges$YEAR_BUILT_027, bridges$OPERATING_RATING_064, bridges$COUNTY_CODE_003, bridges$LOCATION_009,bridges$RAILINGS_036A)
#Grabbing information for the year built, operation rating, the county code of the bridge, location of the bridge, and whether or not it has railings.
head(new.bridges)
```

    ##   bridges.YEAR_BUILT_027 bridges.OPERATING_RATING_064 bridges.COUNTY_CODE_003
    ## 1                   1932                         26.3                      51
    ## 2                   1948                         34.2                     115
    ## 3                   1979                         30.8                     115
    ## 4                   1977                         40.0                       3
    ## 5                   1980                         47.2                       3
    ## 6                   1980                         47.2                       3
    ##          bridges.LOCATION_009 bridges.RAILINGS_036A
    ## 1 '6KM NW OF LAC DU FLAMBEAU'                     0
    ## 2 '10 KM  NE  OF  BOWLER    '                     1
    ## 3 '13 KM  NE  OF  BOWLER    '                     1
    ## 4 '3 KM  EAST  OF  ODANAH   '                     0
    ## 5 '3 KM  NW  OF  ODANAH     '                     0
    ## 6 '2 KM  NW  OF  ODANAH     '                     0
