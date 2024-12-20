---
title: "Workflow-practice"
author: "yuko"
date: "2024-10-18"
output:
  html_document:
    keep_md: true
---


```r
## insert actual code here
data1 = c(2, 5, 3, 6, 8, 12, 9, 25, 8, 10, 16)
mean(data1)
```

```
## [1] 9.454545
```

```r
sd(data1)
```

```
## [1] 6.51711
```

```r
sum(data1)
```

```
## [1] 104
```


## R Markdown

This is an R Markdown practice document. R Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>. 

### Text formatting
Document can be formatted by syntax for header\
- # Header 1 (main title)\
- ## Header 2 (section)\
- ### Header 3 (subsection)\

Text can be emphasized by using italic, bold, strikethrough, or subscript:\
- *italic* or _italic_\
- **bold** or __bold__\
- ~~ strikethrough~~\
- text^superscript^\
- text~subscript~\

Breaks in R Markdown include\
- Line break—to start a new line. Implemented by ending the previous line with a backslash\
- Paragraph break—to start a new paragraph. Implemented by ending the previous paragraph with two spaces.\
- Slide break—to start a new slide in the slide-based output formats (presentations) or a new section in all the other formats. Implemented by inserting a horizontal rule (***) into the document.\
- Page break—to start a new page, in those output formats where it's applicable, e.g., in Microsoft Word. Implemented by inserting the command newpage into the document.\

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:


```r
print("Practicing code chunk")
```

```
## [1] "Practicing code chunk"
```


```r
summary(cars)
```

```
##      speed           dist       
##  Min.   : 4.0   Min.   :  2.00  
##  1st Qu.:12.0   1st Qu.: 26.00  
##  Median :15.0   Median : 36.00  
##  Mean   :15.4   Mean   : 42.98  
##  3rd Qu.:19.0   3rd Qu.: 56.00  
##  Max.   :25.0   Max.   :120.00
```

Rmarkdown is not limited to using only R, but also supports other programming language (see the code chunk drop down) also name each code chunks NOTE: need to install python

```r
print("Hello, World!")
```

```
## [1] "Hello, World!"
```

## Code Chunk options - this information comes from R Markdown Tutorial for beginners in Data Camp
echo=FALSE: the code itself will not be shown in the final document, only its outputs.\
eval=FALSE: the code in the code chunk will not be run.\
include=FALSE: the code chunk will be run but not included in the final document.\
results: the default value is "markup"; other values are:\
  "hide": the code output will be hidden in the final document\
  "hold": the code output will be shown with a delay, only after the whole code chunk is executed\
  "asis": the code output will be passed through without reformatting.\
message=FALSE: the messages produced by the code will not be shown.\
error=FALSE: the errors produced by the code will not be shown.\
warning=FALSE: the warnings produced by the code will not be shown.\
highlight=FALSE: the code will not be highlighted in the final document.\
prompt=TRUE: the > symbol will be added at the beginning of each code line shown in the final document.\


```
## [1] "Practicing code chunk"
```

## Including Plots


### Customize plots in R Marcdown using chunk options
fig.show: the default value is "asis"; other values are:\
  "hide": the plots will be generated but not included in the final document\
  "hold": the plots will be shown with a delay, only after the whole code chunk is executed\
  "animate"—all the plots of the code chunk will be combined into an animation.\
fig.width: the plot width in inches, 7 by default.\
fig.height: the plot height in inches, 7 by default.\
fig.align: the way of aligning plots in the final document, can be "left", "center", or "right".\
fig.cap: a figure caption represented by a character string.\
fig.path: a path to the directory where the plot files created by the code chunk should be stored.\
fig.ext: the extension of the plot files created by the code chunk.\


```r
plot(pressure)
```

![Fig.1. Vapor Pressure of Mercury as a Function of Temperature](Workflow-practice_files/figure-html/pressure-1.png)



Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.
