Sales Prediction(Regression Problem)
-----------------------

Building a predictive model and find out the sales of each product at a particular store.
The model will try to understand the properties of products and stores which play a key role in increasing sales [here](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/).

Installation
----------------------

### Download the data

* Clone this repo to your computer.
* Get into the folder using `cd sales_prediction`.
* Run `mkdir data`.
* Switch into the `data` directory using `cd data`.
* Run  `mkdir raw  processed`.
* Switch into `raw` directory using `cd raw` and download the data files from Analytics Vidhya into the `raw` directory.  
    * You can find the data [here](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/).
    * You'll need to register with Analytics Vidhya to download the data.
    * Download train and test files.
* Switch back into the `sales_prediction` directory using `cd ..`.

### Install the requirements
 
* Install the requirements using `pip install -r requirements.txt`.
    * Make sure you use Python 3.
    * You may want to use a virtual environment for this.

Usage
-----------------------

* Run `mkdir processed` inside `data` directory to create a directory for our processed datasets.
* Run `1-Data_Prep.ipynb`.
    * This performs data preparation, where we look at the structure of the data, missing values and how different variables relate to the target variable. Once we are done with data preparation we move it to `processed` folder.
* Run `EDA's`.
    * These consists of different modeling algorithms to assist in prediction.
        
Model Building
-----------------------

In model building we will use simpler linear models and then move over to more complex models like RandomForest and XGBoost.

* Linear Regression `2-EDA #1`, `2-EDA #2`
* Lasso Regression  `2-EDA #3`
* Ridge Regression  `2-EDA #3`
* RandomForest      `2-EDA #4`
* XGBoost           `2-EDA #5`

### Evaluation Metrics for Regression

The process of model building is not complete without evaluation of model’s performance. That’s why we need an evaluation metric to evaluate our model. Since this is a regression problem, we can evaluate our models using any one of the following evaluation metrics:

* Mean Absolute Error(MAE)
* Mean Squared Error(MSE)
* Root Mean Squared Error(RMSE)