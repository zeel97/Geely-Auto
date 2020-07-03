# Geely-Auto 🚗

### Business Objective
A chinese business automobile company is looking to move into the US Market and start manufacturing there and gain a competitive advantage over the European and US counterparts. They require an analysis and understanding of the factors that affect the pricing of cars in the American market. 
The objectives include:
1. Identifying the variables that affect the price of cars in America
2. Analyse the impact of each feature on the price
3. Recommend possible requirements for Geely Auto to work on

### Model Development
1. Data Cleaning
  1. Convert to relevant Data Types
  2. Format the columns
    1. Split CarName to get Company Name
    2. Delete CarName column (has too many unique values and less likely to contribute to the analysis)
  3. Lower Case all values
2. EDA Analysis
3. Data Preparation
  *Splitting into train and test set
  *Feature Scaling
4. Model Building: Try out 2 different approaches, with and without car companies. With Model 1, the final features are heavily dominated by car company names. Therefore clearly indicating the importance of Brand Image. However, since Geely may not have control over the perception in manufacturing, we attempt another model without car company names to identify other quantitative features that may impact the pricess of the cars. 
    1. Model 1: Inclusive of car companies 
    2. Model 2: Exclusive of car companies
5. Residual Analysis
6. Predicting the Model
7. Model Evaluation: 
    1. R-Squared - 0.823
    2. Adj. R-Squared - 0.817
    3. F-statistic - 136.9
    4. AIC - -375

### Recommendation
1. **Engine Size**: this is one of the most important feature in determining the price. Greater, the better
2. **Engine Type**: avoid OHCV, one better option could be OHCF.
3. **Fuel System**: IDI is a good suggestion. It does not affect the price much though
4. **No.of Cylinders**: avoid 12, choose either 2 or 5. Although looking at the 2 models it seems that 2 has more impact on the price.
5. **Peak RPM**: both the models show that it has some significant on the price of a car
6. **Car length**: along with this, during the analysis it was evident that **curb weight, horsepower & car width** are also important features. Although they were highly correlated to the other features, it is important to note the significance of these features as well


**Concluding Statement**: while our model has given a good insight on the factors that affect the price of cars in the USA, we can always improvise on the model by trying out different regression models such as Linear Regression. Additionally it is clear that the existing feature were more than useful, it could also be enhanced further by adding more derived variables.
    
