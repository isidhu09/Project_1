# COVID-19 Crunchers

NU Data Science Boot Camp: Project 1

Submitted by Harish Korrapati, Britney Washington, Ishanjit Sidhu, Corey Lawson-Enos

## Summary
* Prelminary analysis of COVID-19 death impact on select demograhics in four US states with highest death counts: California, Texas, New York, and Florida. Regression of COVID-19 death counts against vaccination plotted.

## Packages Required
sodapy (Socrata), json, requests, pandas, numpy, matplotlib.pyplot, scipy.stats, census

## API Tokens Required
Save to config.py file as:
* US CDC: appToken = '<token>'
* US Census: api_key = '<token>'

US CDC Token Request: https://data.cdc.gov/login

US Census API Key Request: https://api.census.gov/data/key_signup.html

## Summary Analysis
* Sample demographic data for study states:

![alt text](https://github.com/hvkorrapati/NU_project_1/blob/caaef9c5ccae1a6e5fa9ca6df83c3156460a3cc7/Images/deathct_by_sex.png)
  
![alt text](https://github.com/hvkorrapati/NU_project_1/blob/caaef9c5ccae1a6e5fa9ca6df83c3156460a3cc7/Images/deathct_by_agegrp.png)

* Race/Population Comparison: Since the chi-square values at a confidence level of 95% are much lower than the critical value of 12.6, we conclude that the differences seen across race categories compared to the states' general populations are not statistically significant.
  
* Regression and sample heatmap:
 
![alt text](https://github.com/hvkorrapati/NU_project_1/blob/be2ae9114d61bc14737430a02dee319472254db1/Images/Scatter_Vaccine_vs_Death.png)
 
* Covid/Vaccine Regression: Moderate negative correlation between vaccines and covid deaths at about -.5. As more vaccines are administered death rates trend down.
  
![alt text](https://github.com/hvkorrapati/NU_project_1/blob/be2ae9114d61bc14737430a02dee319472254db1/Images/Scatter_Vaccine_vs_Death_Heat.png)

![alt text](https://github.com/hvkorrapati/NU_project_1/blob/5ef89958a3c418fb5ecb2736058eddf201c6940c/Images/US_County_heatmap.png)
