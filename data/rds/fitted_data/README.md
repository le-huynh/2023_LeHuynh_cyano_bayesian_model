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

## fitted data:
rain = c(250, 375, 475, 600): see `code/get_fitted_data.R`  
- `fit_pc50_logit.rds`, `fit_mcyb50_logit.rds`: climate data = 50-day prior to collection date  


