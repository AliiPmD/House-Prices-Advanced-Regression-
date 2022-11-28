# House Prices Advanced Regression  

#### Hi! I'm Ali (PmD) PourMohammad! This Project is just a warm-up and mostly has an educational and training purpose.
#### Maybe it will be useful for those who are new to this field!

## files:
* `data_description.txt` has information about data
* `train.csv` and `House.csv` are for train and evaluate a model
* `test.csv` doesn't have outcomes and it's for evaluation on the kaggle site
* and `housePricePrediction.ipynp` has codes that I've written to solve this problem

### In this notebook I applied some preprocesses like:
* Drop columns with high outliers
* Drop some data with outlier values
* Drop ID col
* Convert all 'NaN' Values in 14 categorical Columns to 'NOT' (For example : "No Basement" stored as "NaN")
* Drop columns which have most null values
* Convert all categorical columns to numeric:
     ###### In this data, we have three type of categorical columns: 1)Binary 2)Nominal and 3)Ordinal
     ###### I encode ordinal with OrdinalEncoder or .map() func and encode Binary and Nominal with Get_Dummy
     ###### *** Also, ‘MSSubClass’ Column has nominal values but encoded with numbers that may harm model, so I’m going to encode that with Get_dummy too.
* Find correlated columns and drop one of each
* get_dummy all remain categorical columns

##### And finally I've trained a GradientBoostingRegressor model and get 0.945 score.

# Thanks for reading ;)