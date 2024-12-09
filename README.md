# Distributed Lag Models - Application on Temperature-Mortality Associations

A **distributed lag model** is a type of regression model used in econometrics and time series analysis to examine the relationship between a dependent variable and lagged (past) values of an independent variable. These models are especially useful when the effect of an independent variable on the dependent variable is spread over time rather than occurring instantaneously.

## Key Components of Distributed Lag Models

1. **Lagged Variables**:
   - The model includes multiple lagged values of the independent variable as predictors. For example:  
     
     $y_t = \beta_0 + \beta_1 x_t + \beta_2 x_{t-1} + \beta_3 x_{t-2} + \cdots + \epsilon_t$

2. **Lag Structure**:
   - The number of lags considered is determined by the context or through statistical testing. The lag length captures how far back the influence of $x_t$ extends.

3. **Lag Weights**:
   - The coefficients $(\beta_1, \beta_2, \dots)$ indicate the strength and pattern of the lagged effects. They may decay, oscillate, or remain constant over time.
  
## Temperatue-Mortality Associations


## Data

For this work, information about mortality, morbidity, temperature, demographic and influenza incidence was available. Focus was given to the 1995 - 2020 time period.

The data preparation resulted in the construction of data sets for each municipality and district, each with $9\,497$ daily observations, for the time period between 01/01/1995 and 31/12/2020, composed by the following variables:

- ```District``` or ```Municipality``` - District or municipality;
- ```deaths``` - Number of deaths;
- ```deaths_[0,65)``` - Number of deaths for the $[0,65)$ age group; 
- ```deaths_>=65``` - Number of deaths for the $\geq 65$ age group;
- ```tmin``` - Minimum temperature (ºC) (index minimum temperature in the case of districts);
- ```tmean``` - Mean temperature (ºC) (index mean temperature in the case of districts);
- ```tmax``` - Maximum temperature (ºC) (index maximum temperature in the case of districts);
- ```pop_total``` - Annual estimated resident population for the specific municipality or district;
- ```pop_[0,65)``` - Annual estimated resident population aged between 0 and 64 for the specific municipality or district;
- ```pop_>=65``` - Annual estimated resident population aged 65 or over for the specific municipality or district;
- ```Semester``` - Classification between *warm* or *cold* according to the month;
- ```ILI``` - Computed influence like illness incidence.  



