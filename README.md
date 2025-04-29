# Task 4: Classification with Logistic Regression

## Objective
Build a binary classification model using **Logistic Regression** to predict whether a tumor is **malignant** or **benign**, based on cell nuclei features from breast cancer biopsies.

## Tools & Libraries
- Python
- Pandas
- Scikit-learn
- Matplotlib
- NumPy

## 📊 Dataset
**Breast Cancer Wisconsin Diagnostic Dataset**  
- **Source**: Built-in Scikit-learn dataset (`load_breast_cancer`)  
- **Samples**: 569  
- **Features**: 30 numeric features related to tumor characteristics  
- **Target**:  
  - `0` = malignant  
  - `1` = benign  

## 🔁 Workflow

### 1. Load Dataset
- Dataset is directly loaded from `sklearn.datasets`.
- Features (`X`) and labels (`y`) extracted into Pandas DataFrames.

### 2. Preprocessing
- Split into training and test sets (80/20).
- Standardize features using `StandardScaler` for improved convergence.

### 3. Model Training
- Logistic Regression model is trained using default parameters.

### 4. Evaluation Metrics
- **Confusion Matrix**
- **Precision, Recall, F1-Score**
- **ROC Curve**
- **AUC (Area Under the Curve)**

### 5. Threshold Tuning
- Default classification threshold is `0.5`.
- Also tested threshold at `0.3` to observe changes in model sensitivity.
- New predictions evaluated with updated confusion matrix.

### 6. Sigmoid Function Explanation
- Logistic Regression uses the sigmoid function to map linear outputs to probabilities between 0 and 1.
- The sigmoid curve is plotted for visualization.

## Results
- High accuracy and AUC due to well-separated classes.
- ROC curve and classification report help assess performance.
- Lowering threshold improves recall but may increase false positives.
