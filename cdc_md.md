``` r
library(tidyverse)
load("cdc_health.RData")
head(cdc_health, 10)
```

<div class="kable-table">

| gender | race                              | age | weight | height | exercise | health    |
| :----- | :-------------------------------- | --: | -----: | -----: | :------- | :-------- |
| Female | Black                             |  80 |     70 |    157 | No       | Good      |
| Female | White                             |  70 |     49 |    163 | Yes      | Fair      |
| Female | Black                             |  67 |     86 |    165 | Yes      | Good      |
| Female | White                             |  80 |     50 |    152 | No       | Very good |
| Male   | White                             |  71 |    113 |    185 | Yes      | Very good |
| Male   | White                             |  72 |    109 |    188 | Yes      | Excellent |
| Male   | White                             |  77 |     78 |    180 | Yes      | Good      |
| Female | White                             |  71 |     43 |    160 | No       | Poor      |
| Female | White                             |  70 |     59 |    163 | Yes      | Very good |
| Male   | American Indian or Alaskan Native |  55 |     82 |    188 | No       | Poor      |

</div>

``` r
summary(cdc_health)
```

    ##     gender                race             age           weight      
    ##  Male  :174287   White      :281829   Min.   :18.0   Min.   : 23.00  
    ##  Female:198614   Hispanic   : 31126   1st Qu.:42.0   1st Qu.: 68.00  
    ##                  Black      : 27218   Median :59.0   Median : 79.00  
    ##                  Asian      :  8036   Mean   :55.5   Mean   : 82.33  
    ##                  Multiracial:  7673   3rd Qu.:70.0   3rd Qu.: 93.00  
    ##                  Unsure     :  6303   Max.   :80.0   Max.   :281.00  
    ##                  (Other)    : 10716                                  
    ##      height      exercise           health      
    ##  Min.   : 91.0   Yes:273314   Excellent: 59192  
    ##  1st Qu.:163.0   No : 99587   Very good:122985  
    ##  Median :170.0                Good     :118043  
    ##  Mean   :170.1                Fair     : 52954  
    ##  3rd Qu.:178.0                Poor     : 19727  
    ##  Max.   :241.0                                  
    ##
