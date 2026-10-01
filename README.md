# Parkinson's Disease Diagnosis Project
 Classification | Voice Biomarkers | Predictive Modeling
 
**AI-Driven Parkinson’s Disease Detection: A High-Accuracy End-to-End ML Pipeline with External Prediction**

Developed an end-to-end machine learning pipeline for the early detection of Parkinson’s disease (PD) using voice-based biomarkers from the UCI Parkinson’s Disease dataset. The dataset contains 195 voice recordings from 31 individuals (23 with Parkinson’s disease and 8 healthy controls), represented by 22 acoustic features and one binary target variable.

The pipeline was designed & built to prevent data leakage by maintaining a strict separation between training and testing data throughout model development. After an 80/20 stratified train-test split, all preprocessing steps—including feature scaling and class balancing using SMOTE—were performed exclusively on the training data, while the test set remained completely untouched until final model evaluation.

Eight supervised machine learning algorithms were implemented and compared: Logistic Regression (LR), K-Nearest Neighbors (KNN), Decision Tree (DT), Random Forest (RF), Naïve Bayes (NB), Support Vector Machine (SVM), Extreme Gradient Boosting (XGBoost), and a Multi-Layer Perceptron (MLP) neural network. Model selection and performance estimation were conducted using 5-fold Stratified Cross-Validation on the training set, with performance reported as the mean accuracy, precision, recall, F1-score, and ROC-AUC across the five folds.

The MLP neural network achieved the highest mean cross-validation accuracy (92%), outperforming XGBoost (88%) and K-Nearest Neighbors (87%). The finalized models were subsequently evaluated on the untouched 20% test set to assess their generalization performance MLP: 97% test accuracy, test precision (100%) and 98.62% ROC-AUC.The trained pipeline was further demonstrated on a single unseen external voice observation, successfully generating an individual Parkinson’s disease status prediction, demonstrating the practical application of the end-to-end predictive system for non-invasive, AI-powered Parkinson’s disease screening.

This project demonstrates expertise in machine learning pipeline design, data preprocessing, class imbalance handling, cross-validation, comparative model evaluation, and predictive analytics using Python, Pandas, NumPy, Scikit-learn, XGBoost, and Matplotlib. The resulting solution highlights the potential of AI-powered, non-invasive voice analysis to support early Parkinson’s disease screening and clinical decision-making.
