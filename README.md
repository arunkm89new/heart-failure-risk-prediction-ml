🧠 Models Implemented

The following models were trained and evaluated:

Logistic Regression (Baseline & final winner)

Decision Tree

Random Forest

XGBoost

Neural Network (MLP) – comparison only

Neural Networks were included for comparison, but were not the primary focus, as tree-based models and linear models are generally more suitable for tabular medical data.

📈 Evaluation Metrics

Because this is a healthcare problem, model evaluation prioritizes:

Recall → minimize false negatives (missing sick patients)

ROC-AUC → overall class separation

Accuracy and Precision are reported but not primary

🏆 Model Comparison Results
Model Accuracy Precision Recall ROC-AUC
Logistic Regression 0.886 0.872 0.931 0.930
Random Forest 0.880 0.870 0.922 0.931
XGBoost 0.848 0.870 0.853 0.916
Neural Network (MLP) 0.837 0.840 0.873 0.901
Decision Tree 0.815 0.827 0.843 0.877
✅ Final Model Selection

Although ensemble models like Random Forest and XGBoost are generally powerful, Logistic Regression achieved the highest Recall while maintaining a strong ROC-AUC.

🔍 Why Logistic Regression?

Highest Recall → fewest missed heart disease cases

Stable and interpretable

Indicates that the relationship between features and target is largely linear

Safer choice for medical decision support

In healthcare, minimizing false negatives is more critical than maximizing accuracy.

📌 Final Selected Model: Logistic Regression

🧠 Key Learnings

Simple models can outperform complex models on clean, tabular datasets

Model selection should be driven by business/domain risk, not model complexity

Recall is more important than accuracy in medical diagnosis

Neural Networks are not always the best choice for tabular data

Proper experiment tracking and comparison is critical

📌 Conclusion

This project demonstrates an end-to-end supervised learning workflow, emphasizing responsible model selection and domain-aware evaluation.
The final model choice reflects practical ML engineering principles rather than model hype.
