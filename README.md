# Ola-Churn Supervised Learning 

### Problem Statement
To predict drivers that have good probability of leaving based on the driver's details. Churned Driver can lead to Churned Customers as if no of drivers are less in area,

### Insights & Recommendations compared after training using Decision Tree, Random Forest, GBDT, XGBoost, LightGBM

* Churn customers are more in dataset, nearly twice the non churned customers.
* Ages are majorly from 25 to 40. Age 35+ years are more likely to Churn.
* Mostly drivers have income 25000 to 100000. From incomes > 75000, churn customers are seen in more percentage
* We see much more churned customers after 2 years (700 days)
* Ratio of male to female drivers is 60:40. Both are proportionately Churning.
* More income & less business value also increases chances of Churn
* Quarterly ratings & income is increased recently for Churn customers
* Joining designation 1 is more prone to Churn while joining designation 3 retains the drivers more.
* Cities like C20 & C17 have concerning churn rates. Ola should try to retain drivers here.
* High business value drivers have mostly churned which is concerning. Income should be increased proportionately for them.
* While model training, best results for recall were given by LightGBM where we tuned hyperparameters such that we get 97% recall, i.e. Only 10 drivers out of 477 drivers, we were not able to predict that they will Churn.  So, with 97% test accuracy we will be able to predict if driver is about to Churn. We have good enough 84% precision as well. Ola may reach out to these drivers so as to retain them. 
* False Positives (driver not churning & predicted Churning) is something Ola can handle (no harm in extra phone call) but False negatives are critical. 
