# 20210903_Reiff_Metis_Classification_Project
_This repo contains project scoping, MVP concepts, and accompanying analytical documentation/findings for the Metis Classification module commenced Aug 2021_

---
### **Project scope**
* **Background:** Household debt is growing at [alarming](https://www.ceicdata.com/en/indicator/india/household-debt--of-nominal-gdp) rates in India and abroad. Using historical consumer credit data, the Indian government can proactively target citizens at high risk of loan default to offer debt relief programs, with the end goal of stabilizing population financial health. Due to limited government outreach resources, acute identification of the highest-risk individuals is a priority. Additionally, government agencies seek to optimize relief funds, and outreach to individuals not in need of relief should be minimized. Finally, given the staggering amount of consumer credit-related data on-hand, a computationally efficient model is preferable for incremental test observations.  
* **Data & implementation:** This analysis leverages a [public data set](https://www.kaggle.com/subhamjain/loan-prediction-based-on-customer-behavior?select=Training+Data.csv&taskId=5752) of >250k observations and 11 features, including income, car/house ownership, profession, and location for Indian citizens to classify each observation as defaulted or not defaulted (the target classes). Default rates for the entire sample approximate 12%, requiring class balancing to enhance model precision and recall. 
* **Tool/technology requirements:** This analysis employs KNN, logistic regression, and random forest classifiers to assign classes to observations. Visualizations are constructed with Seaborn/Matplotlib.      
* **Objective(s):** This analysis seeks to design a classification model optimized for recall, with F-beta as a benchmark between algorithms. The MVP for this project demonstrates that default-proneness can be determined by the features of the data set superior to the naive expected value of default.      

---
### **Findings/conclusions**
A Random Forest model produces results superior to KNN and logistic regression, as benchmarked by F-beta and ROC-AUC score. Hyperparameter tuning may increase model efficacy and remains further work. 
