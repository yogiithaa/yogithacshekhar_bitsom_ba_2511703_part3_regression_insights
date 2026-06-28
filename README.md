# Part 3: Regression-Based Business Insights & Model Interpretation

## Business Problem Summary

The leadership team of a retail chain wants to understand which factors are most strongly associated with monthly sales performance across stores. The goal is to identify business drivers that can support decisions regarding marketing investment, inventory management, staffing, and regional strategy.

---

## Dataset Description

The dataset contains monthly operational and sales information for retail stores across multiple regions and store types.

### Dependent Variable

* monthly_sales

### Independent Variables Considered

* marketing_spend
* footfall
* avg_discount_pct
* staff_count
* inventory_availability_pct
* competitor_distance_km
* holiday_flag
* customer_rating
* region
* store_type

### Numerical Variables

* marketing_spend
* footfall
* avg_discount_pct
* staff_count
* inventory_availability_pct
* competitor_distance_km
* customer_rating
* monthly_sales
* monthly_profit

### Categorical Variables

* region
* store_type

---

## Data Preparation

The original dataset was preserved in the Original_Data worksheet.

Missing values were identified in:

* customer_rating
* competitor_distance_km

Missing values were replaced using median imputation in the Cleaned_Data worksheet.

The following fields were not used as predictors:

* store_id
* month
* monthly_profit

---

## Regression Approach

Three regression models were evaluated:

### Model 1: Simple Regression

Dependent Variable:

* monthly_sales

Independent Variable:

* marketing_spend

### Model 2: Simple Regression

Dependent Variable:

* monthly_sales

Independent Variable:

* footfall

### Model 3: Multiple Regression

Dependent Variable:

* monthly_sales

Independent Variables:

* marketing_spend
* footfall
* inventory_availability_pct
* region dummy variables

---

## Dummy Variable Approach

The variable region was converted into dummy variables.

Reference Category:

* East

Dummy Variables Created:

* region_North
* region_South
* region_West

East was excluded from the regression equation to avoid the dummy variable trap and multicollinearity.

---

## Model Comparison Summary

| Model   | Variables Used                                                    | R²    |
| ------- | ----------------------------------------------------------------- | ----- |
| Model 1 | Marketing Spend                                                   | 0.167 |
| Model 2 | Footfall                                                          | 0.736 |
| Model 3 | Marketing Spend, Footfall, Inventory Availability, Region Dummies | 0.811 |

The multiple regression model produced the highest explanatory power and was selected as the final model.

---

## Final Model Selected

The multiple regression model was selected because it explains approximately 81.1% of the variation in monthly sales while incorporating multiple business drivers.

---

## Business Recommendation

The analysis suggests that footfall, marketing spend, and inventory availability are positively associated with monthly sales performance.

Management should prioritize:

* Increasing customer traffic
* Maintaining high inventory availability
* Optimizing marketing investment
* Investigating successful practices in South and West regions

---

## Assumptions and Limitations

* Regression identifies association, not causation.
* Important business factors may not be included in the dataset.
* External market conditions are not captured.
* Results should be interpreted as directional evidence rather than proof of cause-and-effect relationships.


