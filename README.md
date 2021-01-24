# Heart Disease UCI Binary Classification
 
Note: Since github only allows for static rendering of notebooks, please go to https://nbviewer.jupyter.org/github/anthonydwan/Heart-Disease-UCI-Binary-Classification/blob/main/Heart%20Disease%20Binary%20Classification.ipynb to review the notebook containing interactive plots and diagrams. 


 
This is a personal side project on predicting heart disease based on various health factors and observations. There are several goals that I would like to achieve in this project: 
* practise feature engineering and feature selection with the hopes of improving machine learning techniques;
* implementing and evaluating different machine learning techniques;
* investigating feature importance - this is particularly useful in healthcare context as we can explain what factors contribute to heart disease and allow better diagnosis and how to take preventive measures. 


## Summary of findings:
1. Binning the features did not contribute to improvement of decision tree models. However, logistic regression may have benefitted from the data transformations as it has performed comparable with more complicated and powerful models such as CatBoost or XGBoost. Another the reason may be stemmed from the simplicity of the dataset which meant that simpler models can perform well. 


2. Feature Importance: 
<p>
<img src="https://github.com/anthonydwan/Heart-Disease-UCI-Binary-Classification/blob/main/barplot%20-%20feature%20importance%20for%20CB.png" width="800" />
</p>

Interesting, we see that 'ca', the number of major vessels colored by flourosopy, is the most important feature in predicting heart disease. 

The second most important factor is 'cp', cheat pain types. 

<p>
<img src="https://github.com/anthonydwan/Heart-Disease-UCI-Binary-Classification/blob/main/shap%20values.png" width="800" />
</p>
The above are visualisation of SHAP Values (an acronym from SHapley Additive exPlanations) which is a break down of a prediction to show the impact of each feature. When the value is greater than 0, it means that the prediction is 1 (that person has heart disease) and vice versa. 
<p><p>
Interestingly, we see that females have an increased change of heart diease than male. While angina and non-anginal pain (chest pain) both contribute to the risk of heart disease, if there are one or less major vassels colored by flourospy and if hemogolbin level is normal, the risk of heart diease is greatly reduced.  
 </p>
