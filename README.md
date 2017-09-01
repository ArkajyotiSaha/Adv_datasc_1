# Adv_datasc_1
Advanced Data Science I Project


My project will be with the data available in Zillow competition. In order to get access to the data one needs to register the competition as a team. After the data is acquired, this is how I wish to proceed with the data analysis:
  1. Exploratory data analysis.
  2. Data imputation to get rid of missing data.
  3. This being a case of spatial data, it will be modeled with a Gaussian process as it provides a rich generalized modelling framework for spatial data. The next step is deciding upon the covariance function (exponential, matern, spherical etc.), that will be used to model the spatial dependence structure among the observations.
  4. The next task is to decide upon the nature of relationship between the outcome and the covarates. The initial trial will be with linear regression. In case, the results are not upto the mark, higher order interaction terms will be included in the model. If inclusion of suffcient number of higher order terms fail to provide significant improvement, I will opt for machine learning algorithms (Random forest, Neural Net etc.) to model the relationship between the covariates and the outcome.
  5. The size of the dataset being in millions, instead of fullgp model a scalable Nearest Neighboour Gaussian Process will be used with a suitble choice of number of nearest neighbiurs (usually limited to 20) in order to take care of the spatial component.
  6. In order to get confidence interval of the estimates, both the Bayesian (MCMC) and the frequentist approach (Bootstrap) will be deployed.
