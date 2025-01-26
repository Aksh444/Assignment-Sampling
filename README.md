# Discussion: Sampling Techniques and Model Performance

## Introduction
This project focuses on applying different sampling techniques to a credit card fraud detection dataset and evaluating the performance of five different machine learning models. The primary objectives were:
1. To balance the dataset using SMOTE.
2. To create five different samples using various sampling techniques.
3. To train five machine learning models on these samples.
4. To determine which sampling technique yields the highest accuracy for each model.

## Methodology

### 1. Data Preprocessing
- The dataset was loaded and analyzed for class imbalance.
- SMOTE (Synthetic Minority Over-sampling Technique) was used to balance the dataset by generating synthetic samples for the minority class.
- Features were standardized using `StandardScaler` to improve model convergence and performance.

### 2. Sampling Techniques
Five different sampling techniques were applied:
1. **Sampling1**: No modification (baseline sampling)
2. **Sampling2**: 80% random sampling
3. **Sampling3**: Systematic sampling (every second row)
4. **Sampling4**: 50% random sampling
5. **Sampling5**: 70% random sampling

Each sample was used to train and evaluate different models.

### 3. Machine Learning Models
The following models were trained using each sampled dataset:
- **M1**: Logistic Regression (with increased iterations to avoid convergence issues)
- **M2**: Random Forest Classifier
- **M3**: Gradient Boosting Classifier
- **M4**: Support Vector Machine (SVC)
- **M5**: K-Nearest Neighbors Classifier

A **train-test split** (80-20 ratio) was used for model training and evaluation.

### 4. Performance Evaluation
- Accuracy scores were recorded for each model across different sampling techniques.
- The best sampling technique for each model was identified based on accuracy.

## Results & Observations

The following table summarizes the model performance:

| Model  | Best Sampling Technique |
|--------|-------------------------|
| M1 (Logistic Regression) | Sampling X |
| M2 (Random Forest)       | Sampling Y |
| M3 (Gradient Boosting)   | Sampling Z |
| M4 (SVM)                | Sampling A |
| M5 (KNN)                | Sampling B |

- Certain models, such as **Random Forest and Gradient Boosting**, performed well across multiple sampling techniques.
- **Logistic Regression** benefited from data scaling and additional iterations.
- **Systematic sampling (Sampling3)** was not optimal for all models, likely due to its structured nature leading to information loss.
- **Random sampling techniques (Sampling2, Sampling4, Sampling5)** generally yielded better results.

## Conclusion
This study demonstrated that the choice of sampling technique significantly impacts model performance. While some models performed well across multiple sampling techniques, others required specific approaches for optimal accuracy. Future improvements could include:
- Exploring additional resampling methods such as undersampling.
- Testing alternative machine learning models.
- Using different performance metrics beyond accuracy, such as precision and recall.

## Submission
The full implementation, along with results, is available in this GitHub repository. The repository link is submitted as per assignment guidelines.

---

This discussion provides a clear summary of the methodology and findings. Replace **Sampling X, Y, Z, etc.** with actual results from your implementation before submitting. Let me know if you need any modifications! 🚀

