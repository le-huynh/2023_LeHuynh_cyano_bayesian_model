# Modeling outputs

This folder contains serialized model objects and related outputs generated 
during statistical modeling.  

These files are not included in this repository because of file size limitations. 
Modeling outputs can be reproduced using the analysis scripts provided in 
the `code/` directory.

# RDS objects
Hurdle Poisson model:  
+ Logistic part: absence probability = env. condition  
+ Poisson part: gene ~ env. condition + (1|Pond)  

## Formula
gene_logit = gene ~ ztemp + zTSI + zrain + (1|Pond),
	 bsence ~ ztemp + zTSI + zrain

gene_temp = gene ~ ztemp + (1|Pond),
         absence ~ ztemp

gene_rain = gene ~ zrain + (1|Pond),
         absence ~ zrain

gene_tsi = gene ~ zTSI + (1|Pond),
        absence ~ zTSI

gene_temp_rain = gene ~ ztemp + zrain + (1|Pond),
	    absence ~ ztemp + zrain

gene_temp_tsi = gene ~ ztemp + zTSI + (1|Pond),
	   absence ~ ztemp + zTSI

gene_rain_tsi = gene ~ zTSI + zrain + (1|Pond),
	   absence ~ zTSI + zrain


## Bayesian models
- `pc*.rds`, `mcyb*.rds`: fitted models using climate data = 50-day prior to collection date, including kfoldic  


