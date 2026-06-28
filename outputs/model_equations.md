# Model Equations

## Simple Regression Model 1

### Equation

Monthly Sales = 560,777.35 + 2.13(Marketing Spend)

### Interpretation

The coefficient suggests that every additional unit of marketing spend is associated with approximately 2.13 additional units of sales.

Marketing spend shows a positive relationship with sales.

---

## Simple Regression Model 2

### Equation

Monthly Sales = 446,410.58 + 35.68(Footfall)

### Interpretation

The coefficient indicates that each additional visitor is associated with approximately 35.68 units of additional sales.

Footfall shows a strong positive relationship with sales.

---

## Multiple Regression Model

### Equation

Monthly Sales

= 131,500

* 1.186(Marketing Spend)

* 33.87(Footfall)

* 2818.21(Inventory Availability %)

* 10,550(region_North)

* 21,940(region_South)

* 17,490(region_West)

---

## Coefficient Interpretation

### Intercept

Represents baseline sales when all predictors equal zero.

### Marketing Spend

Higher marketing expenditure is associated with higher monthly sales.

### Footfall

Footfall is the strongest predictor in the model.

More customer visits are associated with increased sales.

### Inventory Availability

Stores maintaining higher inventory availability tend to achieve stronger sales performance.

### Region Variables

The coefficients represent differences relative to the East region.

---

## Dummy Variable Explanation

Reference Category:

* East

Dummy Variables:

* region_North
* region_South
* region_West

East is omitted from the model to prevent multicollinearity.

Each dummy coefficient measures the difference in sales relative to East after controlling for other variables.

---

## Final Model Selected

Selected Model:

* Multiple Regression Model

Reason for Selection:

* Highest R² value
* Includes multiple business drivers
* Strongest decision-making usefulness
* Better explanatory power than simple regression models
