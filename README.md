# Sales Predictions
## Analysis of Outlet Stores and Making Future Sales Predictions 
#### Author: Kai Dawson-Fischer
### Can Outlet Store Sales be predicted?
Can sales for an Outlet brand be predicted through analyzation of Outlet size, item visibility, etc?
## Data
Data Source:

https://docs.google.com/spreadsheets/d/e/2PACX-1vRN2-Or8bi3tlXj1xnkNU66rebV_AuT-K5pGWjnPLcHL3QtTja1ndIvtea6TSsJHiZD3ZjO2yvxU9Z4/pub?gid=1922513210&single=true&output=csv

Data Dictionary:

![Data Dictionary](https://github.com/G3ntl3g1ant/sales-predictions/blob/main/variable_dictionary.png)

## Methods
- Processed the data by removing duplicates 
- Replaced the missing values in the Item_Weight column with 'Missing' so as to not taint the data
- Replaced the missing values in the Outlet_Size column with the median Outlet_Size so that those missing data could still be counted with the most common variable without biasing the data too much.
- Removed the Outlet_Establishment_Year column because it is unnecessary in the pursuit of Sales Predictions for the Outlet_Sales
- Corrected the values of Item_Fat_Content to gain uniformity in the values presented

## Results
![Outlet Sales Vs Outlet Size](https://github.com/G3ntl3g1ant/sales-predictions/blob/main/maximum_retail_price.png)

Here we can see in the scatter plot above that the majority of sales are coming from the Medium Size Outlets, with the Smaller Outlets coming in 2nd.

![Outlet Sales Vs Item Visibility](https://github.com/G3ntl3g1ant/sales-predictions/blob/main/item_visibility.png)

Here we see the correlation between Outlet_Sales Vs Item_Visibility, organized by Item_Type. Surprising enough, even with less than 19% visibility, the top 3 most sold Item_Types are 'Household', 'Fruits and Vegetables', and 'Baking Goods'.

## Model
The final model that was chosen to be used was the RandomForestRegressor Model.

After processing it and breaking it down, it was the best choice by far.

The R^2 values were found to be:

Training Data: 61% can be explained

Testing Data: 60% can be explained

With an overall RMSE of $1060.31

This is integral, because even with such a margin of error this model can give some insight on future sales, and with that in mind it can also help lower costs on food spoilage.

## Reccomendations:
If this model is used, and used appropriately, it can be a benefit to any company that decides to use it. 

Food spoilage is a major concern for any grocery chain, and if there was a way to even have a guess as to what sales might look like in the future, it can save that company many hard earned dollars and save that many more future headaches. 

## Limitations & Next Steps
This model is not perfect, but it will get you in the right diretion, and with more data coming in everyday, as new methods & new algorithms are created I will add to this model. 

Updating my skill, prowess, and overall ingenuity.


#### For further information:
For any additional questions, please contact kaidawsonfischer2022@gmail.com
