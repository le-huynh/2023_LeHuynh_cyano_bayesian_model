# Modeling outputs

This folder contains serialized model objects and related outputs generated 
during statistical modeling.  

These files are not included in this repository because of file size limitations. 
Modeling outputs can be reproduced using the analysis scripts provided in 
the `code/` directory.

# RDS objects
Hurdle Poisson model:  
+ Poisson part: gene ~ temp + rainfall + TSI + (1|pond)  
+ Logistic part: absence probability = temp + rainfall + TSI  

## Bayesian models
- `pc*_logit.rds`, `mcyb*_logit.rds`: fitted models using climate data = *-day prior to collection date, including kfoldic  
*: 10, 20, 30, 40, 50, 60, 70, 80, 90, 100 days

