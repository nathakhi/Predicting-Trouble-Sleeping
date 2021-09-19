**Background**

Sleep is considered to be one of the major determinants of health.  Inadequate sleep not only disrupts performing daily activities like concentrating on works, memorizing, driving, managing financial affairs but also poses the risk of several physical morbidities including cardiovascular, metabolic, endocrine dysfunction as well as mental health problems like depression or mood disorders when the sleep deprivation is chronic (Medic, Wille, & Hemels, 2017). Several studies have even established the relation between abnormal sleep behavior and mortality. There are several socio-economic, cultural, demographic, and health-related factors that can influence sleep quality. Here, I have tried to seek answers to a number of questions related to poor sleep quality among Canadian population- 


1. Determine some of the important indicators of poor sleep quality,
2. Whether there is difference in trouble sleeping among men and women,  
3. Build ML models to predict the probability of having trouble sleeeping or not.

**Data**

Canadian Community Health Survey (2017-18) accessed via Ryerson Library from Statistics Canada

Target variable:
Trouble going to sleep or staying asleep (renamed as trouble_sleeping)
 
Predictor Variables used:  
- **sociodemographic**: Age, sex, marital status, have kids under 6 years of age, kids 6 to 11 years of age, kids under 12 years of age, immigration status, race  
- **socioeconomic**: Household income, personal income, education level, household size (no. of persons), house ownership  
- **lifestyle**: Smoking, Drinking, BMI, Physical activity indicators  
- **health variables**: Having asthma, COPD, High blood pressure, diabetes, cancer, mood disorder, anxiety disorder, self-reported perception of general and mental health, and satisfaction with life.

**Methods**

- Data Preprocessing  
- Exploratory Data Analysis  
- Hypothesis Testing  
- Machine Learning Classification Models  

**Model Comparison**

Model  | Accuracy 
--------------------------|------------------
Logistic Regression       | 0.6511 
Decision Tree             | 0.6425 
Random Forest             | 0.6445 
KNN                       | 0.5961
Neural Networks(MLP)      | 0.6514

**Conclusion**  

From the model comparison we can see that logistic regression and neural networks models are performing relatively better than other classifiers in terms of clssifying the probabilities of having trouble sleeping based on the selected predictors.

**References**   
- Medic, G., Wille, M., & Hemels, M. E. H. (2017). Short- and long-term health
consequences of sleep disruption. In Nature and Science of Sleep (Vol. 9, pp. 151–161). Dove Medical Press Ltd. https://doi.org/10.2147/NSS.S134864  

- https://towardsdatascience.com/inference-for-categorical-data-9f3c6034aa57    

- **Data source:** Statistics Canada. 2018. Canadian Community Health Survey (CCHS), 2017-2018, (subset compiled from public-use microdata file). Statistics Canada (producer). Using IDLS (distributor). http://janus.ssc.uwo.ca/idls/ (accessed October 16, 2020). 
