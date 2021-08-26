Gesicht das Gesicht
================
Hendrik Jürges
26 8 2021

``` r
## insert your brilliant WORKING code here
head(iris)
```

    ##   Sepal.Length Sepal.Width Petal.Length Petal.Width Species
    ## 1          5.1         3.5          1.4         0.2  setosa
    ## 2          4.9         3.0          1.4         0.2  setosa
    ## 3          4.7         3.2          1.3         0.2  setosa
    ## 4          4.6         3.1          1.5         0.2  setosa
    ## 5          5.0         3.6          1.4         0.2  setosa
    ## 6          5.4         3.9          1.7         0.4  setosa

``` r
iris |> 
  lm(formula = Sepal.Length~Sepal.Width) |> 
  arm::display()
```

    ## lm(formula = Sepal.Length ~ Sepal.Width, data = iris)
    ##             coef.est coef.se
    ## (Intercept)  6.53     0.48  
    ## Sepal.Width -0.22     0.16  
    ## ---
    ## n = 150, k = 2
    ## residual sd = 0.83, R-Squared = 0.01
