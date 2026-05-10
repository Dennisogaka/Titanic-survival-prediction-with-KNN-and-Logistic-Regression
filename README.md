## Titanic Survival Prediction: KNN vs. Logistic Regression
This project implements a machine learning pipeline to predict passenger survival on the Titanic. The core focus is a comparative analysis between a linear model (**Logistic Regression**) and a distance-based model (**K-Nearest Neighbors**).

## Project Overview
Using the classic Titanic dataset, this project explores data preprocessing, feature scaling, and model evaluation. The goal is to determine which algorithm better handles the non-linear relationships present in the passenger data (Age, Fare, etc.).

## Tech Stack
**_Language:_** 
- Python

**_Libraries:_**
- Pandas & NumPy for data manipulation.
- Seaborn & Matplotlib for data visualization.
- Scikit-Learn for model training and evaluation.

## Workflow
_**1. Data Cleaning:**_ 

- Handled missing values for 'age' and 'embarked' columns.

_**2. Feature Engineering:**_

- Label Encoding for categorical variables (sex, embarked).

- Standard Scaling to normalize features (essential for KNN performance).

_**3. Model Training:**_

- Logistic Regression: A baseline linear classifier.

- KNN (k=5): A neighbor-based classifier.

_**4. Evaluation:**_ 
- Used Confusion Matrices to visualize True Positives, True Negatives, and misclassifications.
  
## Model Performance
In regards to accuracy, the KNN model(79.21%) outperformed Logistic Regression(76.97%).
While KNN had higher accuracy, Logistic Regression showed different trade-offs in precision.

### KNN Performance
<img width="550" height="455" alt="image" src="https://github.com/user-attachments/assets/224098ed-404b-4ae7-b3bb-a2872b344af2" />


### Logistic Regression Performance
<img width="550" height="455" alt="image" src="https://github.com/user-attachments/assets/b12720a8-2ea2-4b75-b202-2fe48a803cfc" />

## Conclusion
While _**Logistic Regression**_ is _**highly interpretable**_, _**KNN**_ provided better _**predictive power**_ for this specific dataset. This suggests that the _**survival boundaries**_ in the Titanic data are likely _**non-linear**_, allowing the _**neighbor-based approach**_ to capture patterns that a straight-line formula might miss.
