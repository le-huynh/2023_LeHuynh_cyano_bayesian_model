# Modeling outputs

This folder contains serialized model objects and related outputs generated 
during statistical modeling.  

These files are not included in this repository because of file size limitations. 
Modeling outputs can be reproduced using the analysis scripts provided in 
the `code/` directory.

# RDS objects
Hurdle Poisson model:  
+ Poisson part: gene ~ temp + rainfall + TSI + (1|pond)  
+ Logistic part: absence probability = constant  

## Bayesian models
- `mcyB2var.rds`: fitted model for mcyB, using 2 predictors (air temperature + TSI), climate data = 30-day prior to collection date  
- `pc*.rds`, `mcyb*.rds`: fitted models using climate data = *-day prior to collection date, including kfoldic  
*: 5, 10, 15, 20, 25, 30 days

## fitted data:
rain = c(200, 300, 400, 500): see `code/get_fitted_data.R`  
- `fitpc30.rds`, `fitmc30.rds`: climate data = 30-day prior to collection date  
- `fitpc25.rds`, `fitmc25.rds`: climate data = 25-day prior to collection date  


