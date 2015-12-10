# R language code in markdown page

## Analysis of Tomato plant growth under different light condition

Three plants ( A, B and C ) were exposed to different Light conditions

Plant A was exposed to 12 hours of light every day
Plant B was exposed to 8 hours of light every day
Plant C was exposed to 4 hours of light every day


We draw some interesting plots here in this Repo.


```r
library(ggplot2);
library(dplyr);
library(stringr);


dim(tomatodata)
```

```
## Error in eval(expr, envir, enclos): object 'tomatodata' not found
```

```r
names(tomatodata)
```

```
## Error in eval(expr, envir, enclos): object 'tomatodata' not found
```

```r
head(tomatodata)
```

```
## Error in head(tomatodata): object 'tomatodata' not found
```

```r
str(tomatodata)
```

```
## Error in str(tomatodata): object 'tomatodata' not found
```


##Plot of Tomato plant height


```r
g1 <- ggplot(data = tomatodata, aes(x=tomatodata$"Days", y=tomatodata$"Height", color=tomatodata$Height))
```

```
## Error in ggplot(data = tomatodata, aes(x = tomatodata$Days, y = tomatodata$Height, : object 'tomatodata' not found
```

```r
g1 = g1 + geom_point();
```

```
## Error in eval(expr, envir, enclos): object 'g1' not found
```

```r
g1 <- g1 + labs(title="Tomato Plant Height", x="No. of Days", y="Height")
```

```
## Error in eval(expr, envir, enclos): object 'g1' not found
```

```r
print(g1)
```

```
## Error in print(g1): object 'g1' not found
```

## plot of Height Vs Leaves


```r
g2 <- ggplot(data = tomatodata, aes(x=tomatodata$"Height", y=tomatodata$"Leaves", color=tomatodata$Height))
```

```
## Error in ggplot(data = tomatodata, aes(x = tomatodata$Height, y = tomatodata$Leaves, : object 'tomatodata' not found
```

```r
g2 = g2 + geom_point();
```

```
## Error in eval(expr, envir, enclos): object 'g2' not found
```

```r
g2 <- g2 + labs(title="Height Vs Leaves", x="Height", y="Leaves")
```

```
## Error in eval(expr, envir, enclos): object 'g2' not found
```

```r
g2
```

```
## Error in eval(expr, envir, enclos): object 'g2' not found
```

## Plot of Tomato Plant leaves


```r
g3 <- ggplot(data = tomatodata, aes(x=tomatodata$"Days", y=tomatodata$"Leaves", 
color= tomatodata$Height, horizontal='true'))
```

```
## Error in ggplot(data = tomatodata, aes(x = tomatodata$Days, y = tomatodata$Leaves, : object 'tomatodata' not found
```

```r
g3 = g3 + geom_point();
```

```
## Error in eval(expr, envir, enclos): object 'g3' not found
```

```r
g3 <- g3 + labs(title="Tomato Plant Leaves", x="No. of Days", y="Leaves")
```

```
## Error in eval(expr, envir, enclos): object 'g3' not found
```

```r
g3
```

```
## Error in eval(expr, envir, enclos): object 'g3' not found
```

## Box Plot


```r
b <-plot(tomatodata$Plant, tomatodata$Height)
```

```
## Error in plot(tomatodata$Plant, tomatodata$Height): object 'tomatodata' not found
```

```r
b
```

```
## Error in eval(expr, envir, enclos): object 'b' not found
```
