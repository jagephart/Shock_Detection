# Shock_Detection
Function to identify shocks in time series

This function was used in Gephart et al. (2017) to detect shocks in time series. 

This method is inspired by a method commonly used to identify outliers in exploratory spatial statistics. This enables shock detection based on deviations in the autocorrelation . The approach is adaptable from spatial to temporal analysis because of the equivalence of the theoretical form of some autocorrelation coefficients between these types of data. The autocorrelation coefficient is an empirical representation of the relationship between temporal measures of production. Deviations identify localized instabilities in the autocorrelation which, conceptually, represent sudden disruptions of the seafood production. Specifically, shocks were identified as outlier deviations, or points with high Cook’s D values (>0.35), in a regression of the residuals and lag-1 residuals from a lowess fit of the time series with a smoother span of 2/3. The threshold of 0.35 was selected by comparing the total number of shocks identified to the threshold and selecting the point where the curve became relatively flat (see Supplementary Figure 1).


Gephart JA, Deutsch L, Pace ML, Troell M, Seekell DA. Shocks to fish production: Identification, trends, and consequences. Global environmental change. 2017 Jan 1;42:24-32.
