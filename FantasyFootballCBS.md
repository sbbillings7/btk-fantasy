---
title: "CBS Fantasy Football League"
author: "Stephen Billings"
date: "October 26, 2017"
output: github_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = FALSE)


library("readxl")
library(dplyr)
fantasy <- read_xlsx("FantasyFootball.xlsx")
StephenBillings <- filter(fantasy, Team == "Stephen's Oneders",)
AdamKahn <- filter(fantasy, Team == "Ghengis Kahn")
GlennBlackmon <- filter(fantasy, Team == "Mo Money, Mo Problems")
BrianKelso <- filter(fantasy, Team == "See You at the Top")
GreyDavis <- filter(fantasy, Team == "Hangin Brains")
MattMendat <- filter(fantasy, Team == "Cleveland Steamers")
JoeHamrick <- filter(fantasy, Team == "Dizzy Pumpkins")
MattKing <- filter(fantasy, Team == "Kings Lohr")
BradLance <- filter(fantasy, Team == "Dirty Fours")
ChadMorrow <- filter(fantasy, Team == "Danny White")
JacobKahn <- filter(fantasy, Team == "Smashing Blumpkins")
WayneHewett <- filter(fantasy, Team == "Highway to Hell")


```


# [Our Fantasy League](http://btk.football.cbssports.com/home)

![](http://fantasy.img.cbssports.com/C/football/leagues/ltk/btk/images/league-logo/2C47DEB6-A9B9-11E7-A65D-5D48377CD9D0-640x800.jpg)

*****


# Glenn Blackmon
```{r Blackmon, echo = FALSE}
filter(GlennBlackmon[, -5])
```
***
# Brian Kelso
```{r Kelso, echo = FALSE}
filter(BrianKelso[,-5])
```
***
# Adam Kahn 
```{r Kahn1, echo = FALSE}
filter(AdamKahn[,-5])
```
***
# Grey Davis
```{r Davis, echoe = FALSE}
filter(GreyDavis[,-5])
```
***
# Matt Mendat
```{r Mendat, echo = FALSE}
filter(MattMendat[,-5])
```

# Joe Hamrick
```{r Hamrick, echo = FALSE}
filter(JoeHamrick[,-5])
```
***
# Matt King
```{r King, echo = FALSE}
filter(MattKing[,-5])
```

# Brad Lance
```{r Lance, echo = FALSE}
filter(BradLance[,-5])
```
***
# Chad Morrow
```{r Morrow, echo = FALSE}
filter(ChadMorrow[-5])
```

# Wayne Hewett
```{r Hewett, echo = FALSE}
filter(WayneHewett[,-5])
```
***
# Jacob Kahn & Austin Bradshaw
```{r Kahn2, echo = FALSE}
filter(JacobKahn[,-5])
```
***
# Stephen Billings
```{r Billings, echo = FALSE}
filter(StephenBillings[,-5])
```
***
Stephen Billings' team costs `r sum(StephenBillings[,4])`