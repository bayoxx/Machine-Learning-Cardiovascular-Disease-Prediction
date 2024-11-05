# Machine Learning
## Regression: Cardiovascular Disease Prediction

**Description**  
This project aimed to predict the 10-year risk of coronary heart disease (CHD) using demographic, behavioural, and medical data. Cardiovascular diseases are a leading cause of mortality globally, and early detection is crucial in preventive healthcare. This predictive model targets middle-aged individuals—a critical age group for heart disease risk—to aid in identifying high-risk individuals for timely interventions.

**Objective**  
The primary objective was to develop a logistic regression model to accurately predict the likelihood of a patient developing CHD within 10 years. The focus was on optimizing the model to balance sensitivity and specificity, thereby improving the model's utility in a clinical setting.  

**Methodology**  
1. **Data Preprocessing**: Missing values were imputed, and features were scaled for consistency.
2. **Exploratory Data Analysis (EDA)**: Statistical and visual analysis provided insights into the distribution of risk factors and their relationships with CHD.
3. **Addressing Imbalance**: Since the dataset had an underrepresented CHD-positive class, the SMOTE (Synthetic Minority Over-sampling Technique) method was used to balance the dataset, ensuring that the model was not biased toward the majority class.
4. **Model Development**: Logistic regression was chosen for its interpretability and effectiveness with binary classification. Optimal threshold analysis was used to set a threshold for CHD prediction based on maximizing the F1 Score, Precision, and Recall.
5. **Evaluation Metrics**: Model performance was evaluated using Accuracy, Precision, Recall, F1 Score, and ROC-AUC Score to understand predictive quality comprehensively.

**Tools & Technologies**  
- **Programming Languages**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Development Environment**: Jupyter Notebook

**Insights**  
- **Demographic Patterns**: Age, cholesterol levels, and blood pressure were among the key indicators of increased risk for CHD. 
- **Behavioral & Medical Influences**: Lifestyle factors such as smoking and diabetes history showed a strong correlation with CHD risk.
- **Optimal Threshold Selection**: Adjusting the decision threshold improved the model’s sensitivity to CHD cases, thereby increasing recall at the expense of some precision, making it better suited for identifying at-risk individuals.

**Challenges & Solutions**  
- **Class Imbalance**: The imbalance in CHD cases posed a challenge in model accuracy. Using SMOTE helped balance the classes, which in turn improved recall for CHD cases without overly compromising precision.
- **Threshold Selection**: The default 0.5 probability threshold did not yield the best recall-precision balance. Optimal threshold analysis based on ROC-AUC curves enabled better customization of the model to achieve healthcare objectives, allowing flexibility between higher recall or precision based on the clinical goal.


## Outcome
The general outcome of the Cardiovascular Disease Prediction project showed that, through data preprocessing, resampling techniques (such as SMOTE), and logistic regression modeling, it was possible to create a predictive model for the 10-year risk of coronary heart disease (CHD) with reasonable accuracy and interoperability. 

The optimal threshold analysis allowed for a more balanced evaluation of precision and recall, tailored to identify higher-risk individuals while minimizing false positives. This model serves as a foundational step in understanding the risk profile of middle-aged adults in the dataset, providing actionable insights that can be further refined for preventive healthcare strategies.

**Recommendations**  
- **Further Testing with Advanced Models**: Consider testing with ensemble methods or tree-based algorithms like Random Forest or Gradient Boosting to improve model performance and handle non-linear relationships.
- **Feature Engineering**: Additional health indicators, such as physical activity levels and genetic information, could provide more comprehensive insights and improve prediction accuracy.
- **Implementation in a Clinical Workflow**: Deploying this model as a decision-support tool can help clinicians identify high-risk patients, promoting early intervention and personalized healthcare strategies. 

This project underscores the importance of leveraging machine learning in preventive healthcare, showcasing my capability to handle real-world data imbalances, optimize model performance, and derive actionable insights that can be utilized for strategic decision-making in health risk management.

I have attached the .ipynb file to this repository. I have also attached the report, check [here](https://github.com/bayoxx/Machine-Learning-Cardiovascular-Disease-Prediction/blob/main/cardiovascular.pdf)

Thank you for your time.


