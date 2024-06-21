# ML-Techniques-for-Dental-Diseases

### Project Description

This project is centered on predicting dental diseases using machine learning techniques. It is divided into two main parts: data preprocessing and model building.

#### Data Preprocessing (Data_PreprocessinP1.ipynb)

The data preprocessing phase is crucial for preparing the dataset for machine learning applications. The steps involved include:

1. **Data Loading**: The dataset is loaded, and initial checks for missing values are performed.
2. **Feature Exploration**: Various features are analyzed to understand their relationship with the target variable, which is the presence of dental disease.
   - For example, an exploration of the 'toothpaste usage' column revealed a higher frequency of dental problems among regular users, indicating that this feature might not be very informative for prediction and could be dropped.
   - Another feature examined is the 'total minutes used to brush teeth' (tfb), with categories like 1 minute, 2 minutes, and 3 minutes.
3. **Column Dropping**: Redundant or irrelevant columns are identified and removed. For instance, the 'smoke' column is dropped in favor of the more detailed 'smoke in a day' column, and 'smokeless tobacco' is also removed due to its overlap with smoking habits.
4. **Data Conversion**: All categorical data types are converted to numeric values to facilitate machine learning algorithms.
5. **Feature Correlation**: The correlation between different features is checked to understand their interrelationships and their potential impact on the model.

#### Machine Learning Model Building (MLPart-1.ipynb)

In this phase, various machine learning models are applied to the preprocessed data to predict dental diseases. The key steps include:

1. **Model Selection**: Different classifiers are chosen, including Linear SVC, KNeighbors Classifier, RandomForestClassifier, and Logistic Regression.
2. **Train-Test Split**: The dataset is split into training and testing sets to evaluate model performance.
3. **Model Comparison**: A function is created to compare the accuracy of different models easily.
4. **Evaluation Metrics**: Models are evaluated using ROC curves and confusion matrices, with a focus on understanding false positives and false negatives.
5. **Hyperparameter Tuning**: RandomizedSearchCV is employed for tuning the parameters of RandomForestClassifier and Logistic Regression to improve performance.
6. **Visualization**: The results of hyperparameter tuning are visualized using ROC curves.
7. **Final Model Evaluation**: The results of GridSearchCV and RandomizedSearchCV are compared, and models are evaluated using confusion matrices and classification reports.
8. **Model Saving**: The final, optimized model is saved for future use.

By integrating thorough data preprocessing with robust model building and evaluation techniques, this project aims to develop an effective tool for predicting dental diseases, thereby aiding in better diagnosis and treatment planning.
