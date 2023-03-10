Objective:
1. To predict melting efficiency of AM process.


Methodology:
1. 
### Preprocession steps

|Sr.No.| Step | Option 1 | Option 2 |
|---| --- | --- | --- |
|1| Missing value | info | isnull |
|2| Encoding |  |  |
|3| Outlier | boxplot |  |
|4| Feature scaling |  |  |
|5| Imbalance |  |  |

2. Build 
a) Linear regression model by OLS in statsmodel
b) Gaussian process model
c) XGB regressor
d) MLP

3. 
### Checks

|Sr.No.| Step | Requirement | Decision |
|---| --- | --- | --- |
|1| Adjusted R2 | >70 | Ok |
|2| Check p-value | <0.05 | Ok  |
|3| No heteroscadicity |  | Ok |
|4| No auto correlation | Durbin-Watson test 1.5-2.5 | Not Ok |
|5| No multi collinearity | VIF<5 | Ok |

Results and Conclusion:
1. GP algorithm provides more accurate results than XGB and ANN.
