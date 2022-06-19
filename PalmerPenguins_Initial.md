---
title: "Palmer Penguins Initial Analysis"
author: "Katie Duryea"
format: html
editor: visual
execute:
  keep-md: true
---



## Palmer Penguins

This is a test of Quarto functionality using the Palmer Penguins package.


::: {.cell}

```{.r .cell-code}
 library(tidyverse)
```

::: {.cell-output .cell-output-stderr}
```
Warning: replacing previous import 'lifecycle::last_warnings' by
'rlang::last_warnings' when loading 'pillar'
```
:::

::: {.cell-output .cell-output-stderr}
```
Warning: replacing previous import 'lifecycle::last_warnings' by
'rlang::last_warnings' when loading 'tibble'
```
:::

::: {.cell-output .cell-output-stderr}
```
Warning: replacing previous import 'lifecycle::last_warnings' by
'rlang::last_warnings' when loading 'hms'
```
:::

::: {.cell-output .cell-output-stderr}
```
── Attaching packages ─────────────────────────────────────── tidyverse 1.3.0 ──
```
:::

::: {.cell-output .cell-output-stderr}
```
✓ ggplot2 3.3.5     ✓ purrr   0.3.4
✓ tibble  3.1.4     ✓ dplyr   1.0.7
✓ tidyr   1.1.3     ✓ stringr 1.4.0
✓ readr   2.0.1     ✓ forcats 0.5.0
```
:::

::: {.cell-output .cell-output-stderr}
```
── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
x dplyr::filter() masks stats::filter()
x dplyr::lag()    masks stats::lag()
```
:::

```{.r .cell-code}
    library(palmerpenguins)
    
    penguins %>% head()
```

::: {.cell-output .cell-output-stdout}
```
# A tibble: 6 × 8
  species island bill_length_mm bill_depth_mm flipper_length_… body_mass_g sex  
  <fct>   <fct>           <dbl>         <dbl>            <int>       <int> <fct>
1 Adelie  Torge…           39.1          18.7              181        3750 male 
2 Adelie  Torge…           39.5          17.4              186        3800 fema…
3 Adelie  Torge…           40.3          18                195        3250 fema…
4 Adelie  Torge…           NA            NA                 NA          NA <NA> 
5 Adelie  Torge…           36.7          19.3              193        3450 fema…
6 Adelie  Torge…           39.3          20.6              190        3650 male 
# … with 1 more variable: year <int>
```
:::
:::


This code loads the `palmerpenguins` package and displays the top (or `head`) of the dataset.
