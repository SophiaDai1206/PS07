PS07
================

## Section 01

``` r
library(moderndive)
library(Stat2Data)
library(ggplot2)
data("Cereal")
data("CrabShip")
```

![crab](README_files/figure-gfm/crab1.png)

## The relationship between Oxygen consumption and crabs’ mass

``` r
ggplot(CrabShip, aes(x=Mass,y=Oxygen, color= Noise))+ 
  geom_point() +
geom_parallel_slopes(se=FALSE, formula=y~x)
```

![](README_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->
