# Model Comparison

## Overview

Three regression models were evaluated to determine which factors best explain monthly sales performance.

---

## Model 1: Marketing Spend

### Variables

Dependent Variable:

* monthly_sales

Independent Variable:

* marketing_spend

### Results

* R² = 0.167
* Marketing spend statistically significant
* Positive relationship with sales

### Business Usefulness

Marketing spend appears associated with sales growth. However, the model explains only a limited portion of sales variation.

### Limitations

* Ignores store traffic
* Ignores operational factors
* Does not account for regional differences

---

## Model 2: Footfall

### Variables

Dependent Variable:

* monthly_sales

Independent Variable:

* footfall

### Results

* R² = 0.736
* Strong statistical significance
* Strong positive relationship

### Business Usefulness

Footfall is a major predictor of sales performance and provides strong explanatory power.

### Limitations

* Does not explain why footfall differs across stores
* Ignores marketing and inventory effects

---

## Model 3: Multiple Regression

### Variables

Dependent Variable:

* monthly_sales

Independent Variables:

* marketing_spend
* footfall
* inventory_availability_pct
* region_North
* region_South
* region_West

### Results

* R² = 0.811
* Highest explanatory power
* Multiple statistically significant predictors

### Significant Variables

* Footfall
* Marketing Spend
* Inventory Availability
* South Region
* West Region

### Business Usefulness

This model provides the strongest support for decision-making because it incorporates multiple operational and market factors simultaneously.

### Limitations

* Does not include local economic conditions
* Does not capture management quality
* Does not prove causation

---

## Final Model Selection

The multiple regression model was selected because it achieved the highest R² value and provides the most comprehensive view of factors associated with monthly sales performance.
