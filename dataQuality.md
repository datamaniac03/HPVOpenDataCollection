# Data quality and exploratory graphical analysis report for HPV Open Data Collection Project

Velber Xavier, PhD velberxavier@gmail.com
Jose Eduardo Santana, MSc candidate jes@ic.ufal.br
Jacson Barros, MSc Jacsonv@ffm.br
Joao Ricardo Vissoci, PhD candidate jnv4@duke.edu
Amrapali Zaveri, MSc, PhD candidate zaveri@informatik.uni-leipzig.de
Ricardo Pietrobon, MD, PhD rpietro@duke.edu

<!---
Velber and Jose Eduardo, do you guys have institutional email addresses? if so, please add them above
-->



```
## Error: file 'Hmisc' is not an OS X binary package
```

```
## Error: package 'e1071' could not be loaded
```


<!---
Velber, please take the previous line where it says label and then create labels for each one of the variables you have in your data set. please write them in simple Portuguese and then convert them to English using Google translate. please talk with Jose Eduardo if you have any questions
-->

## Introduction
The main objective of this report is to provide a 24/7 snapshop at the data quality behind the HPV Open Data Collection Project. This includes not only the original data set collected under Dr. Xavier in Maceio, Brazil, but also any additional data sets brought in from other registries, prospective studies, as well as Linked Open Data sources.

Methodological details about the study can be found at [HPV Open Data Collection Project](site)

## Data Description
Below is a full list of variables along with their class (variable type according to the R language) and alternative responses. Most of the variable names should be intuitive, but a full dictionary is also described below:


```
## Error: unused argument(s) (exclude.missing = FALSE)
```


A description of missing values is provided in the Figure below, where missing values are presented in yellow.
![plot of chunk unnamed-chunk-3](figure/unnamed-chunk-3.png) 

```
##       Age data Samples Agemenarche age1sex numbersexpartners parity
## 1       1    1       1           1       1                 1      1
## Total   0    0       0           0       0                 0      0
##       abortion1 abortion2 pregnancy agefirstbirth oralsex anasex
## 1             1         1         1             0       0      0
## Total         0         0         0             1       1      1
##       contraceptive STD smoke alcohol polymerase Total
## 1                 0   0     0       0          0     1
## Total             1   1     1       1          1     1
```


## Data Quality

Below is a series of graph representations regarding data quality control. Firste set o graphs show the ... gaphs. These graphs aim to indicate ... . These graphs were created with the qcc package (link) from R Language Open Software.


```
## Error: subscript out of bounds
```

![plot of chunk unnamed-chunk-4](figure/unnamed-chunk-4.png) 


bla bla bla


```
## Error: subscript out of bounds
```

```
## Error: subscript out of bounds
```


bla bla bla


```
## Error: object 'obj1' not found
```


## Data Association

Figures regarding associations between variables from the HPV Open Design Data collection projetc are presente below. First set of figures show the the comparison of ... (put numeric variables) between subjects with postivie and negative polymerase values (Checar com Velber).


```
## Error: argument is of length zero
```

```
## Error: argument is of length zero
```

```
## Error: argument is of length zero
```

```
## Error: argument is of length zero
```

```
## Error: argument is of length zero
```

```
## Error: argument is of length zero
```

```
## Error: argument is of length zero
```


Below is an application of the MINE (maximal Information-based Nonparametric Exploration) algorithm from the Science article (Detecting Novel Association in Large Data Sets)[http://www.sciencemag.org/content/334/6062/1518.abstract?ijkey=cRCIlh2G7AjiA&keytype=ref&siteid=sci]. See also (http://www.exploredata.net/)[http://www.exploredata.net/]. This application was used to explore the associations between variables inside the dataset. Variables with highe values of linear relation (MIC-definition)  as well as the analysis of non-lnear associations (MAS - Definition) are shown in figures below.

## Problem with MINE, need to add the data set to the working directory. 
## Any ideia how we can bring the results from mine into the .rmd file as a table?

```
## **********************************************************
## MINE version 1.0.1d
## Copyright 2011 by David Reshef and Yakir Reshef.
## 
## This application is licensed under a Creative Commons
## Attribution-NonCommercial-NoDerivs 3.0 Unported License.
## See
## http://creativecommons.org/licenses/by-nc-nd/3.0/ for
## more information.
## **********************************************************
## 
## 
## input file = hpv.csv
## analysis style = allpairs
## results file name = 'hpv.csv,allpairs,cv=0.0,B=n^0.6,Results.csv'
## print status frequency = every 100 variable pairs
## status file name = 'hpv.csv,allpairs,cv=0.0,B=n^0.6,Status.txt'
## alpha = 0.6
## numClumpsFactor = 15.0
## debug level = 0
## required common values fraction = 0.0
## garbage collection forced every 2147483647 variable pairs
## reading in dataset...
```

```
## Error: java.io.FileNotFoundException: hpv.csv (No such file or directory)
```

```
## Error: need finite 'xlim' values
```

```
## geom_smooth: method="auto" and size of largest group is <1000, so using
## loess. Use 'method = x' to change the smoothing method.
```

```
## geom_smooth: method="auto" and size of largest group is <1000, so using
## loess. Use 'method = x' to change the smoothing method.
```

```
## Error: missing value where TRUE/FALSE needed
```

```
## Loading required package: rgl
```

```
## Error: rgl package missing
```

