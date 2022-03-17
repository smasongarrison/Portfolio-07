Bracket
================
AwesomePie1453 & Mason
16 March, 2022

### Part 3

## The Bracket!

Awesome, now just knit this document/run the code and it will generate
the winners. Be sure to fill your bracket out starting in each round
with the West region, then the East, then the South, then the Midwest.

``` r
Weighted_Probabilities <- function(PT1, team_name_1, PT2, team_name_2){Pbin = (PT1 *100)/(PT1*100 + PT2*100)
gameoutcome <- print(rbinom(1, 1, prob=Pbin))
if(gameoutcome){
  print(paste0(team_name_1," Beats ",team_name_2))
return(c(PT1, team_name_1))
}else{
    print(paste0(team_name_2," Beats ",team_name_1))
return(c(PT2,team_name_2))
}
}
```

### Round of 64 Winners

``` r
library(TeachingDemos)
```

    ## Warning: package 'TeachingDemos' was built under R version 4.1.3

``` r
library(tidyverse)


char2seed('EricWillLose',set=FALSE) %>%
set.seed()
```

``` r
W1 <- Weighted_Probabilities(Gonzaga, "Gonzaga", Georgia_State, "Georgia St.")
```

    ## [1] 1
    ## [1] "Gonzaga Beats Georgia St."

``` r
W2 <- Weighted_Probabilities(Boise_State, "Boise State", Memphis, "Memphis")
```

    ## [1] 1
    ## [1] "Boise State Beats Memphis"

``` r
W3 <- Weighted_Probabilities(UConn, "UConn", New_Mesico_State, "New Mexico State")
```

    ## [1] 0
    ## [1] "New Mexico State Beats UConn"

``` r
W4 <- Weighted_Probabilities(Arkansas, "Arkansas", Vermont, "Vermont")
```

    ## [1] 1
    ## [1] "Arkansas Beats Vermont"

``` r
W5 <- Weighted_Probabilities(Alabama, "Alabama", Rutgers, "Rutgers")
```

    ## [1] 1
    ## [1] "Alabama Beats Rutgers"

``` r
W6 <- Weighted_Probabilities(Texas_Tech, "Texas Tech", Montana_State, "Montana State")
```

    ## [1] 1
    ## [1] "Texas Tech Beats Montana State"

``` r
W7 <- Weighted_Probabilities(Michigan, "Michigan", Davidson, "Davidson")
```

    ## [1] 1
    ## [1] "Michigan Beats Davidson"

``` r
W8 <- Weighted_Probabilities(Duke, "Duke", CS_Fullerton, "CS Fullerton")
```

    ## [1] 1
    ## [1] "Duke Beats CS Fullerton"

``` r
W9 <- Weighted_Probabilities(Baylor, "Baylor", Norfolk_State, "Norfolk State")
```

    ## [1] 1
    ## [1] "Baylor Beats Norfolk State"

``` r
W10 <- Weighted_Probabilities(North_Carolina, "University of North Carolina", Marquette, "Marquette")
```

    ## [1] 0
    ## [1] "Marquette Beats University of North Carolina"

``` r
W11 <- Weighted_Probabilities(Saint_Marys, "St. Marys", Indiana, "Indiana")
```

    ## [1] 0
    ## [1] "Indiana Beats St. Marys"

``` r
W12 <- Weighted_Probabilities(UCLA, "UCLA", Akron, "Akron")
```

    ## [1] 1
    ## [1] "UCLA Beats Akron"

``` r
W13 <- Weighted_Probabilities(Texas, "Texas", Virginia_Tech, "Virginia Tech")
```

    ## [1] 1
    ## [1] "Texas Beats Virginia Tech"

``` r
W14 <- Weighted_Probabilities(Purdue, "Purdue", Yale, "Yale")
```

    ## [1] 1
    ## [1] "Purdue Beats Yale"

``` r
W15 <- Weighted_Probabilities(Murray_State, "Murray State", San_Fransisco, "San Fransisco")
```

    ## [1] 1
    ## [1] "Murray State Beats San Fransisco"

``` r
W16 <- Weighted_Probabilities(Kentucky, "Kentucky", Saint_Peters, "Saint Peters")
```

    ## [1] 1
    ## [1] "Kentucky Beats Saint Peters"

``` r
W17 <- Weighted_Probabilities(Arizona, "Arizona", Bryant, "Bryant")
```

    ## [1] 1
    ## [1] "Arizona Beats Bryant"

``` r
W18 <- Weighted_Probabilities(Seton_Hall, "Seton Hall", TCU, "TCU")
```

    ## [1] 1
    ## [1] "Seton Hall Beats TCU"

``` r
W19 <- Weighted_Probabilities(Houston, "Houston", UAB, "UAB")
```

    ## [1] 0
    ## [1] "UAB Beats Houston"

``` r
W20 <- Weighted_Probabilities(Illinois, "Illinois", Chattanooga, "Chattanooga")
```

    ## [1] 1
    ## [1] "Illinois Beats Chattanooga"

``` r
W21 <- Weighted_Probabilities(Colorado_State, "Colorado State", Michigan, "Michigan")
```

    ## [1] 1
    ## [1] "Colorado State Beats Michigan"

``` r
W22 <- Weighted_Probabilities(Tennessee, "Tennessee", Longwood, "longwood")
```

    ## [1] 1
    ## [1] "Tennessee Beats longwood"

``` r
W23 <- Weighted_Probabilities(Ohio_State, "Ohio State", Loyola_Chicago, "Loyola Chicago")
```

    ## [1] 1
    ## [1] "Ohio State Beats Loyola Chicago"

``` r
W24 <- Weighted_Probabilities(Villanova, "Villanova", Delaware, "Delaware")
```

    ## [1] 1
    ## [1] "Villanova Beats Delaware"

``` r
W25 <- Weighted_Probabilities(Kansas, "Kansas", Texas_Southern, "Texas Southern")
```

    ## [1] 1
    ## [1] "Kansas Beats Texas Southern"

``` r
W26 <- Weighted_Probabilities(San_Diego_State, "San Diego State", Creighton, "Creighton")
```

    ## [1] 1
    ## [1] "San Diego State Beats Creighton"

``` r
W27 <- Weighted_Probabilities(Iowa, "Iowa", Richmond, "Richmond")
```

    ## [1] 1
    ## [1] "Iowa Beats Richmond"

``` r
W28 <- Weighted_Probabilities(Providence, "Providence", SDSU, "South Dakota State")
```

    ## [1] 1
    ## [1] "Providence Beats South Dakota State"

``` r
W29 <- Weighted_Probabilities(LSU, "LSU", Iowa_State, "Iowa State")
```

    ## [1] 1
    ## [1] "LSU Beats Iowa State"

``` r
W30 <- Weighted_Probabilities(Wisconsin, "Wisconsin", Colgate, "Colgate")
```

    ## [1] 1
    ## [1] "Wisconsin Beats Colgate"

``` r
W31 <- Weighted_Probabilities(USC, "USC", Miami_FL, "Miami Florida")
```

    ## [1] 0
    ## [1] "Miami Florida Beats USC"

``` r
W32 <- Weighted_Probabilities(Auburn, "Auburn", Jacksonville_State, "Jacksonville State")
```

    ## [1] 1
    ## [1] "Auburn Beats Jacksonville State"

### Round of 32 Winners

``` r
W33 <- Weighted_Probabilities(as.numeric(W1[1]), W1[2], as.numeric(W2[1]), W2[2])
```

    ## [1] 1
    ## [1] "Gonzaga Beats Boise State"

``` r
W34 <- Weighted_Probabilities(as.numeric(W3[1]), W3[2], as.numeric(W4[1]), W4[2])
```

    ## [1] 0
    ## [1] "Arkansas Beats New Mexico State"

``` r
W35 <- Weighted_Probabilities(as.numeric(W5[1]), W5[2], as.numeric(W6[1]), W6[2])
```

    ## [1] 0
    ## [1] "Texas Tech Beats Alabama"

``` r
W36 <- Weighted_Probabilities(as.numeric(W7[1]), W7[2], as.numeric(W8[1]), W8[2])
```

    ## [1] 0
    ## [1] "Duke Beats Michigan"

``` r
W37 <- Weighted_Probabilities(as.numeric(W9[1]), W9[2], as.numeric(W10[1]), W10[2])
```

    ## [1] 1
    ## [1] "Baylor Beats Marquette"

``` r
W38 <- Weighted_Probabilities(as.numeric(W11[1]), W11[2], as.numeric(W12[1]), W12[2])
```

    ## [1] 0
    ## [1] "UCLA Beats Indiana"

``` r
W39 <- Weighted_Probabilities(as.numeric(W13[1]), W13[2], as.numeric(W14[1]), W14[2])
```

    ## [1] 0
    ## [1] "Purdue Beats Texas"

``` r
W40 <- Weighted_Probabilities(as.numeric(W15[1]), W15[2], as.numeric(W16[1]), W16[2])
```

    ## [1] 0
    ## [1] "Kentucky Beats Murray State"

``` r
W41 <- Weighted_Probabilities(as.numeric(W17[1]), W17[2], as.numeric(W18[1]), W18[2])
```

    ## [1] 1
    ## [1] "Arizona Beats Seton Hall"

``` r
W42 <- Weighted_Probabilities(as.numeric(W19[1]), W19[2], as.numeric(W20[1]), W20[2])
```

    ## [1] 1
    ## [1] "UAB Beats Illinois"

``` r
W43 <- Weighted_Probabilities(as.numeric(W21[1]), W21[2], as.numeric(W22[1]), W22[2])
```

    ## [1] 0
    ## [1] "Tennessee Beats Colorado State"

``` r
W44 <- Weighted_Probabilities(as.numeric(W23[1]), W23[2], as.numeric(W24[1]), W24[2])
```

    ## [1] 0
    ## [1] "Villanova Beats Ohio State"

``` r
W45 <- Weighted_Probabilities(as.numeric(W25[1]), W25[2], as.numeric(W26[1]), W26[2])
```

    ## [1] 1
    ## [1] "Kansas Beats San Diego State"

``` r
W46 <- Weighted_Probabilities(as.numeric(W27[1]), W27[2], as.numeric(W28[1]), W28[2])
```

    ## [1] 1
    ## [1] "Iowa Beats Providence"

``` r
W47 <- Weighted_Probabilities(as.numeric(W29[1]), W29[2], as.numeric(W30[1]), W30[2])
```

    ## [1] 1
    ## [1] "LSU Beats Wisconsin"

``` r
W48 <- Weighted_Probabilities(as.numeric(W31[1]), W31[2], as.numeric(W32[1]), W32[2])
```

    ## [1] 0
    ## [1] "Auburn Beats Miami Florida"

### Sweet 16 Winners

``` r
W49 <- Weighted_Probabilities(as.numeric(W33[1]), W33[2], as.numeric(W34[1]), W34[2])
```

    ## [1] 1
    ## [1] "Gonzaga Beats Arkansas"

``` r
W50 <- Weighted_Probabilities(as.numeric(W35[1]), W35[2], as.numeric(W36[1]), W36[2])
```

    ## [1] 0
    ## [1] "Duke Beats Texas Tech"

``` r
W51 <- Weighted_Probabilities(as.numeric(W37[1]), W37[2], as.numeric(W38[1]), W38[2])
```

    ## [1] 0
    ## [1] "UCLA Beats Baylor"

``` r
W52 <- Weighted_Probabilities(as.numeric(W39[1]), W39[2], as.numeric(W40[1]), W40[2])
```

    ## [1] 1
    ## [1] "Purdue Beats Kentucky"

``` r
W53 <- Weighted_Probabilities(as.numeric(W41[1]), W41[2], as.numeric(W42[1]), W42[2])
```

    ## [1] 1
    ## [1] "Arizona Beats UAB"

``` r
W54 <- Weighted_Probabilities(as.numeric(W43[1]), W43[2], as.numeric(W44[1]), W44[2])
```

    ## [1] 0
    ## [1] "Villanova Beats Tennessee"

``` r
W55 <- Weighted_Probabilities(as.numeric(W45[1]), W45[2], as.numeric(W46[1]), W46[2])
```

    ## [1] 0
    ## [1] "Iowa Beats Kansas"

``` r
W56 <- Weighted_Probabilities(as.numeric(W47[1]), W47[2], as.numeric(W48[1]), W48[2])
```

    ## [1] 0
    ## [1] "Auburn Beats LSU"

### Elite 8 Winners

``` r
W57 <- Weighted_Probabilities(as.numeric(W49[1]), W49[2], as.numeric(W50[1]), W50[2])
```

    ## [1] 1
    ## [1] "Gonzaga Beats Duke"

``` r
W58 <- Weighted_Probabilities(as.numeric(W51[1]), W51[2], as.numeric(W52[1]), W52[2])
```

    ## [1] 0
    ## [1] "Purdue Beats UCLA"

``` r
W59 <- Weighted_Probabilities(as.numeric(W53[1]), W53[2], as.numeric(W54[1]), W54[2])
```

    ## [1] 0
    ## [1] "Villanova Beats Arizona"

``` r
W60 <- Weighted_Probabilities(as.numeric(W55[1]), W55[2], as.numeric(W56[1]), W56[2])
```

    ## [1] 0
    ## [1] "Auburn Beats Iowa"

### Final Four Winners

``` r
W61 <- Weighted_Probabilities(as.numeric(W57[1]), W57[2], as.numeric(W58[1]), W58[2])
```

    ## [1] 1
    ## [1] "Gonzaga Beats Purdue"

``` r
W62 <- Weighted_Probabilities(as.numeric(W59[1]), W59[2], as.numeric(W60[1]), W60[2])
```

    ## [1] 1
    ## [1] "Villanova Beats Auburn"

### Championship Winner

``` r
W63 <- Weighted_Probabilities(as.numeric(W61[1]), W61[2], as.numeric(W62[1]), W62[2])
```

    ## [1] 1
    ## [1] "Gonzaga Beats Villanova"

Thanks for using this bracket generator, hope you win!
