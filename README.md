Credit Risk Analysis Report Summary

In this comprehensive analysis, the efficacy of machine learning models for credit risk classification was thoroughly examined. The primary objective was to construct a model capable of discerning the creditworthiness of borrowers based on historical lending activity data, differentiating between low-risk loans (0) and high-risk loans (1).

Analysis Stages:

Data Preparation: The lending_data.csv dataset was loaded, and labels (y) were derived from the "loan_status" column, while features (X) were created from the remaining columns.

Model Building: An initial Logistic Regression model was employed to predict credit risk. Subsequently, the model was fitted first with the original data and then with resampled data, addressing class imbalance using RandomOverSampler.

Model Evaluation: Model performance was assessed through the generation of confusion matrices and classification reports. Key metrics such as balanced accuracy, precision, and recall scores were calculated.

Results:

Original Data Model

Balanced Accuracy Score: 0.9520
Confusion Matrix:
True Negatives (0): 18,663
False Positives: 102
True Positives (1): 563
False Negatives: 56
Classification Report:
Precision (0): 1.00
Precision (1): 0.85
Recall (0): 0.99
Recall (1): 0.91
Resampled Data Model

Balanced Accuracy Score (Resampled Model): 0.9937
Confusion Matrix (Resampled Model):
True Negatives (0): 18,649
False Positives: 116
True Positives (1): 615
False Negatives: 4
Classification Report (Resampled Model):
Precision (0): 1.00
Precision (1): 0.84
Recall (0): 0.99
Recall (1): 0.99
Summary:

Both machine learning models demonstrated robust performance. The original data model achieved a commendable balanced accuracy score of 0.9520, indicating solid predictive capabilities for both low and high-risk loans. However, the resampled data model showcased a remarkable improvement, reaching a balanced accuracy score of 0.9937, signifying exceptional performance in identifying both loan categories.

The resampled model, with its superior performance, not only ensures high accuracy but also minimizes the risk of misclassifying high-risk loans. Notably, the heightened recall score for high-risk loans (1) in the resampled model is particularly advantageous for a lending service, enhancing the ability to correctly identify a larger proportion of high-risk loans and consequently reducing potential losses.





