---
title       : Kaggle Mobile Ad Competition
subtitle    : 1st Cut of Analysis
author      : Abhishek Kapoor
job         : Mobile Ad Competition
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides


---

## Back-ground

> 1.Hi friends, we take this competition as an opportunity to learn R and to build an architecture around R and big data

> 2.We are using Slidify and R Markdown for reporting

> 3.This competition is hosted on Kaggle - (http://www.kaggle.com/c/avazu-ctr-prediction)

> 4.Libraries we will be using are - ff,ffbase,ffbase2,ggplot2,tidyr,lubridate 

---

## Correspondence Map using R - Eigen values

> 1. Packages - FactoMineR


```r
library(FactoMineR)
author=read.csv("Sample.csv",row.names="X")
```

```
## Warning: cannot open file 'Sample.csv': No such file or directory
```

```
## Error: cannot open the connection
```

```r
ca2<- CA(author,graph = FALSE)
```

```
## Error: cannot coerce class ""function"" to a data.frame
```

```r
ca2$eig
```

```
## Error: object 'ca2' not found
```

---

## Correspondence Map Coordinates


```r
head(ca2$col$coord)
```

```
## Error: object 'ca2' not found
```

```r
head(ca2$row$coord)
```

```
## Error: object 'ca2' not found
```

---

## Correspondence Map Plot


```r
plot(ca2)
```

```
## Error: object 'ca2' not found
```

---

## Correspondence Map for end users

> 1. Now here is the link where user can easily upload the data (brand assoication data) and correspondence map will be generated in just fraction of seconds
> 2. Now user don't have to worry of running R codes, loading data or arranging the data in particular format for SPSS run. Simply upload the data and see the results
> 3. Here is the link https://kapoorabhishek.shinyapps.io/PerceptualMap/
> 4. Happy Plotting
