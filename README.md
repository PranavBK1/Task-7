 Breast Cancer Classification using SVM
 Project Overview

Used Breast Cancer Wisconsin (Diagnostic) dataset from Kaggle.

Performed preprocessing, scaling, and dimensionality reduction (PCA → 2D) for visualization.

Trained Support Vector Machines (SVM) with Linear and RBF kernels.

 Steps Performed

Load & Prepare Data

Removed irrelevant columns (id, Unnamed: 32).

Encoded diagnosis → Malignant=1, Benign=0.

Standardized features with StandardScaler.

Reduced to 2 components using PCA for plotting decision boundaries.

Model Training

SVM with Linear Kernel.

SVM with RBF Kernel.

Visualization

Plotted decision boundaries for both kernels using 2D PCA-transformed data.

Hyperparameter Tuning

Tuned C and gamma using GridSearchCV (5-fold cross-validation).

Evaluation

Used cross_val_score for final accuracy estimation.

📊 Results

Linear Kernel Accuracy: 0.991

RBF Kernel Accuracy:  0.982

Best Params from GridSearchCV:'C': 10, 'gamma': 0.01, 'kernel': 'rbf'
