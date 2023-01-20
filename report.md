HW 1, CS 625, Spring 2023
================
Alekhya Puppala
Jan 19, 2023

## Git, GitHub

1.  *What is your GitHub username?*

alekhyap06

2.  *What is the URL of your remote GitHub repo (created through
    Mr. Kennedy’s exercises)?*

<https://github.com/alekhyap06/Datavizualisation-01239677-.git>

## R

The command below will load the tidyverse package. If you have installed
R, RStudio, and the tidyverse package, it should display a list of
loaded packages and their versions.

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.2 ──
    ## ✔ ggplot2 3.4.0      ✔ purrr   1.0.1 
    ## ✔ tibble  3.1.8      ✔ dplyr   1.0.10
    ## ✔ tidyr   1.2.1      ✔ stringr 1.5.0 
    ## ✔ readr   2.1.3      ✔ forcats 0.5.2 
    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()

## R Markdown

1.  *Create a bulleted list with at least 3 items*

- Fruits
- Vegetables
- Chocolates

2.  *Write a single paragraph that demonstrates the use of italics,
    bold, bold italics, code, and includes a link. The paragraph does
    not have to make sense.*

My name is *Alekhya Puppala*

My name is **Alekhya Puppala**

My name is ***Alekhya Puppala***

My name is `Alekhya Puppala`

My favorite search engine is [Duck Duck Go](https://duckduckgo.com).

3.  *Create a level 3 heading*

### This is level 3 heading

## R

#### Data Visualization Exercises

1.  (Q2) *How many rows are in mpg? How many columns?*

There are 234 rows and 11 columns.

``` r
ggplot2::mpg
```

    ## # A tibble: 234 × 11
    ##    manufacturer model      displ  year   cyl trans drv     cty   hwy fl    class
    ##    <chr>        <chr>      <dbl> <int> <int> <chr> <chr> <int> <int> <chr> <chr>
    ##  1 audi         a4           1.8  1999     4 auto… f        18    29 p     comp…
    ##  2 audi         a4           1.8  1999     4 manu… f        21    29 p     comp…
    ##  3 audi         a4           2    2008     4 manu… f        20    31 p     comp…
    ##  4 audi         a4           2    2008     4 auto… f        21    30 p     comp…
    ##  5 audi         a4           2.8  1999     6 auto… f        16    26 p     comp…
    ##  6 audi         a4           2.8  1999     6 manu… f        18    26 p     comp…
    ##  7 audi         a4           3.1  2008     6 auto… f        18    27 p     comp…
    ##  8 audi         a4 quattro   1.8  1999     4 manu… 4        18    26 p     comp…
    ##  9 audi         a4 quattro   1.8  1999     4 auto… 4        16    25 p     comp…
    ## 10 audi         a4 quattro   2    2008     4 manu… 4        20    28 p     comp…
    ## # … with 224 more rows

1.  (Q4) *Make a scatterplot of hwy vs cyl.*

``` r
ggplot(data = mpg) + 
geom_point(mapping = aes(x = cyl, y = hwy))
```

![](report_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

#### Workflow: basics Exercises

1.  (Q2) *Tweak each of the following R commands so that they run
    correctly (`library(tidyverse)` is correct):*

``` r
library(tidyverse)
ggplot(dota = mpg) + 
  geom_point(mapping = aes(x = displ, y = hwy))

fliter(mpg, cyl = 8)

filter(diamond, carat > 3)
```

## Google Colab

1.  *What are the URLs of your Google Colab notebooks (both Python and
    R)?*

Python :
<https://colab.research.google.com/drive/1xblJgiGYKtn8nKpo-gG2sK2jk2buX_3f?usp=sharing>

R :
<https://colab.research.google.com/drive/1BGU0BWsGQSqNygA8iwz6wY0Pn6TcPym-?usp=sharing>

## Tableau

*Insert your the image of your final bar chart here*

![salesincentral](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/salesincentral.png)

1.  *What conclusions can you draw from the chart?*

The sales of technology have risen from 2019 to 2022 and the sales of
furniture have remained more or less the same.

## Observable and Vega-Lite

### A Taste of Observable

1.  *In the “New York City weather forecast” section, try replacing
    `Forecast: detailedForecast` with `Forecast: shortForecast`. Then
    press the blue play button or use Shift-Return to run your change.
    What happens?*

When we change the Forecast:detailedForecast to
Forecast:shortForecast,we observe few minor details.

1.  *Under the scatterplot of temperature vs. name, try replacing
    `markCircle()` with `markSquare()`. Then press the blue play button
    or use Shift-Return to run your change. What happens? How about
    `markPoint()`?*

Under the scatterplot of temperatute vs name, when we replace
‘markCircle()’ with markSquare(), the plot points which were in the form
of circle changed to square. When we replace markSquare() to
markPoint(), the square point plot in the scatterplot turns to points.

![square](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/images/%20square.jpeg)

![point](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/images/point.jpeg)

1.  *Under “Pick a location, see the weather forecast”, pick a location
    on the map. Where was the point you picked near?*

latitude -122.27

longitude 37.87

1.  *The last visualization on this page is a “fancy” weather chart
    embedded from another notebook. Click on the 3 dots next to that
    chart and choose ‘Download PNG’. Insert the PNG into your report.*

![chart!](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/images/chart.png)

### Charting with Vega-Lite

`markCircle()`

1.  *Pass an option of `{ size: 200 }` to `markCircle()`.*

![size200!](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/images/size200.jpeg)

1.  *Try `markSquare` instead of `markCircle`.*

![marksquare](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/images/marksquare.png)

1.  *Try `markPoint({ shape: 'diamond' })`.*

![diamond](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/images/diamond.png)

`vl.x().fieldQ("Horsepower")`, …

1.  *Change `Horsepower` to `Acceleration`*

![horsepower!](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/images/horsepower.png)

1.  *Swap what fields are displayed on the x- and y-axis*

![swap!](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/images/swap.png)

`vl.tooltip().fieldN("Name")`

1.  *Change `Name` to `Origin`.*

Another example, `count()`

1.  *Remove the `vl.y().fieldN("Origin")` line.*

![countofrecords!](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/images/countofrecords.png)

1.  *Replace `count()` with `average("Miles_per_Gallon")`.*

![Average!](/Users/alekhyapuppala/Desktop/Datavizualisation-01239677-/images/Average.png)

## References

*Every report must list the references that you consulted while
completing the assignment. If you consulted a webpage, you must include
the URL.*

- Insert Reference 1,
  <https://r4ds.had.co.nz/workflow-basics.html#practice>
- Reference 2,
  <https://colab.research.google.com/drive/165dTuQy5P7cgG8QqZMuLWP02LD9fLpLJ#scrollTo=qJAKN6380cJc>
- Reference 3, <https://observablehq.com/@tomb/a-taste-of-observable>
- Reference 4, <https://www.tableau.com/academic/students>
- Reference 5, <https://r4ds.had.co.nz/workflow-basics.html#practice>
- Reference 6,
  <https://colab.research.google.com/drive/165dTuQy5P7cgG8QqZMuLWP02LD9fLpLJ#scrollTo=s8aeChJ4_pgz>
