drrecr (DR Recr)
================

drrecr (DR Recr) is a set of tools for evaluating (reconciling) a demand response DR event. There are three tools: 1. Classify similar days 2. Define a demand response 3. Evaluate the demand response event using several methods. Methods include: + 10 prior similar days average + 2 hour prior minimum + 30 minute prior minimum + 5 minute prior minimum

``` r
#Check for similar days 
similar_days(time_series_data) 

#DR Event Definition
event_1 <- dr_event(ymd_hm("2015 3 19 9:50"), hours(3), energy, Time)

#Use output of dr_event to evaluate the event
eval_event(event_1)
```

Use the devtools package to install:

``` r
devtools::install_github("sabrooks/drrecr")
```
