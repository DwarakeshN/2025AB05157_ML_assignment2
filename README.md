1. PROBLEM STATEMENT

The goal of this project is to classify celestial objects observed in the Sloan Digital Sky Survey (SDSS) into one of three categories:
  1. STAR
  2. GALAXY
  3. QSO (Quasar)

Using their astrophysical and photometric properties such as magnitudes (u, g, r, i, z), redshift, and spatial coordinates.

2. DATASET DESCRIPTION

Dataset: Stellar Classification Dataset – SDSS17
Source: Kaggle (https://www.kaggle.com/datasets/fedesoriano/stellar-classification-dataset-sdss17)
Rows: 100,000
Attributes: 17
Target column: class
Classes: "STAR", "GALAXY", "QSO"

Features include:
  1. Photometric magnitudes: u, g, r, i, z
  2. Redshift
  3. Right ascension (alpha) and declination (delta)
  4. Run data (run_ID, cam_col, etc.)

3. MODELS USED

The following models have been implemented:
  1. Logistic Regression
  2. Decision Tree Classifier
  3. K-Nearest Neighbors
  4. Naive Bayes
  5. Random Forest Classifier
  6. XGBoost Classifier

And each model is evaluated using:
  1. Accuracy
  2. Precision
  3. Recall
  4. F1 Score
  5. MCC (Matthews Correlation Coefficient)
  6. AUC (One-vs-Rest, macro-averaged)

Model	Accuracy	Precision	Recall	F1 Score	MCC	AUC
Logistic Regression	0.9571	0.9545	0.9482	0.9506	0.9241	0.988
Decision Tree	0.967	0.9612	0.9631	0.9621	0.9417	0.9716
KNN	0.9271	0.9347	0.9035	0.9179	0.8693	0.9662
Naive Bayes	0.7256	0.7873	0.6403	0.6026	0.507	0.9314
Random Forest	0.9807	0.9809	0.9742	0.9774	0.9656	0.995
XGBoost	0.9772	0.9762	0.9715	0.9737	0.9595	0.9958
