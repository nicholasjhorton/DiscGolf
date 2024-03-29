
<!-- README.md is generated from README.Rmd. Please edit that file -->

# DiscGolf package

The goal of this package is to provide an example of how to create a
data package in R.

It uses Nick’s example from the DataIsPlural website to tell people
about approved discs for disc golf.

See <https://youtu.be/-VHYLgEBzNc> for a Youtube video and the files in
<https://github.com/nicholasjhorton/DiscGolf/tree/master/DiscGolf_files>
for more information.

## Installation

Want to try it? You can install the package from
[GitHub](https://github.com/) with:

``` r
# install.packages("remotes")
remotes::install_github("nicholasjhorton/DiscGolf")
```

## Example

This could be where you provide a basic example which shows you how to
solve a common problem:

``` r
library(DiscGolf)
summary(DiscGolf)
#>  approved_date           class              diameter      flexibility   
#>  Min.   :1964-01-01   Length:1260        Min.   :21.00   Min.   : 0.56  
#>  1st Qu.:2006-04-12   Class :character   1st Qu.:21.10   1st Qu.: 7.37  
#>  Median :2013-07-06   Mode  :character   Median :21.20   Median : 8.96  
#>  Mean   :2009-10-08                      Mean   :21.46   Mean   : 8.76  
#>  3rd Qu.:2017-03-23                      3rd Qu.:21.50   3rd Qu.:10.66  
#>  Max.   :2020-10-03                      Max.   :27.60   Max.   :12.27  
#>                                                          NA's   :2      
#>      height      manufacturer          model             rim_depth    
#>  Min.   :1.300   Length:1260        Length:1260        Min.   :1.100  
#>  1st Qu.:1.700   Class :character   Class :character   1st Qu.:1.100  
#>  Median :1.800   Mode  :character   Mode  :character   Median :1.200  
#>  Mean   :1.893                                         Mean   :1.285  
#>  3rd Qu.:2.000                                         3rd Qu.:1.400  
#>  Max.   :3.800                                         Max.   :2.800  
#>                                                                       
#>  rim_thickness      weight     
#>  Min.   :0.30   Min.   :174.3  
#>  1st Qu.:1.20   1st Qu.:175.1  
#>  Median :1.60   Median :176.0  
#>  Mean   :1.59   Mean   :177.7  
#>  3rd Qu.:2.00   3rd Qu.:178.5  
#>  Max.   :2.60   Max.   :200.0  
#>  NA's   :1
head(DiscGolf)
#>   approved_date class diameter flexibility height
#> 1    2020-10-03  <NA>     21.2        7.95    1.6
#> 2    2020-09-29  <NA>     21.3       11.02    1.4
#> 3    2020-09-29  <NA>     21.3       10.68    1.8
#> 4    2020-09-29  <NA>     21.4        5.11    1.6
#> 5    2020-09-29  <NA>     21.0        6.70    1.9
#> 6    2020-09-29  <NA>     21.2        9.66    2.1
#>                          manufacturer                     model rim_depth
#> 1                         Yikun Discs           Qi (, Qiong Qi)       1.1
#> 2 Viking Discs (IP-Agency Finland Oy)                      Odin       1.1
#> 3 Viking Discs (IP-Agency Finland Oy)                    Fenrir       1.1
#> 4                   Lone Star Molding The Dillard Midrange Md-1       1.2
#> 5                   Lone Star Molding              Penny Putter       1.5
#> 6               Innova Champion Discs                    Animal       1.3
#>   rim_thickness weight
#> 1           2.3  176.0
#> 2           2.3  176.8
#> 3           2.0  176.8
#> 4           1.3  177.6
#> 5           1.1  174.3
#> 6           1.0  176.0
sessionInfo()
#> R version 4.3.1 (2023-06-16)
#> Platform: aarch64-apple-darwin20 (64-bit)
#> Running under: macOS Ventura 13.6
#> 
#> Matrix products: default
#> BLAS:   /Library/Frameworks/R.framework/Versions/4.3-arm64/Resources/lib/libRblas.0.dylib 
#> LAPACK: /Library/Frameworks/R.framework/Versions/4.3-arm64/Resources/lib/libRlapack.dylib;  LAPACK version 3.11.0
#> 
#> locale:
#> [1] en_US.UTF-8/en_US.UTF-8/en_US.UTF-8/C/en_US.UTF-8/en_US.UTF-8
#> 
#> time zone: America/New_York
#> tzcode source: internal
#> 
#> attached base packages:
#> [1] stats     graphics  grDevices utils     datasets  methods   base     
#> 
#> other attached packages:
#> [1] DiscGolf_0.1.0
#> 
#> loaded via a namespace (and not attached):
#>  [1] compiler_4.3.1    fastmap_1.1.1     cli_3.6.1         tools_4.3.1      
#>  [5] htmltools_0.5.6   rstudioapi_0.15.0 yaml_2.3.7        rmarkdown_2.25   
#>  [9] knitr_1.44        xfun_0.40         digest_0.6.33     rlang_1.1.1      
#> [13] evaluate_0.22
```

Last updated October 11, 2023
