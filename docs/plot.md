
# (PART) Preamble {-}

# Plots

Short little intro chapter

## Plotting causes error

Trying to "Build Book"" with this plot causes an error.  Removing the plot book builds fine.


```r
library(tidyverse)
#> -- Attaching packages ------------------------------------------------- tidyverse 1.2.1 --
#> v ggplot2 2.2.1     v purrr   0.2.4
#> v tibble  1.4.2     v dplyr   0.7.4
#> v tidyr   0.8.0     v stringr 1.3.0
#> v readr   1.1.1     v forcats 0.3.0
#> -- Conflicts ---------------------------------------------------- tidyverse_conflicts() --
#> x dplyr::filter() masks stats::filter()
#> x dplyr::lag()    masks stats::lag()

ggplot(data = mpg) + 
  geom_point(mapping = aes(x = displ, y = hwy, color = class))
```



\begin{center}\includegraphics[width=0.7\linewidth]{plot_files/figure-latex/unnamed-chunk-2-1} \end{center}


However, if you "Knit" it will build just fine.
