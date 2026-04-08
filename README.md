Genomic Prediction using SNP Data and Machine Learning
Overview
This project demonstrates how machine learning can be applied to genomic (SNP) data to predict a quantitative trait and identify important genetic markers.
A simulated dataset is used to mimic real-world genomic selection scenarios, where a subset of SNPs influences the trait.
Objectives
Simulate SNP genotype data (0, 1, 2 encoding)
Generate a quantitative trait influenced by selected SNPs
Train a machine learning model (Random Forest)
Evaluate model performance using R² score
Identify important SNPs using feature importance
Compare predicted SNPs with true causal SNPs
Methodology
Data Simulation
Generated 500 samples with 300 SNPs
Selected a subset of SNPs as true causal variants
Added noise to simulate realistic biological variation
Model Training
Used RandomForestRegressor
Split data into training and testing sets (80/20)
Evaluation
Model performance measured using R² score
Feature Importance
Extracted SNP importance from the trained model
Validation
Compared top predicted SNPs with true SNPs
Results
Model: Random Forest Regressor
R² Score: ~0.63
Successfully identified multiple true SNPs
SNP Importance Visualization
Model Performance (Actual vs Predicted)
The scatter plot shows that predicted values follow the general trend of the actual values, indicating that the model captures the underlying relationship between SNPs and the trait.
Some deviation is expected due to noise in the simulated dataset.
Key Insight
The model effectively captures the relationship between selected SNPs and the trait, despite the presence of noise. Feature importance analysis successfully highlights the most influential SNPs.
Technologies Used
Python
NumPy
Pandas
Scikit-learn
Matplotlib
How to Run
Install dependencies:
pip install numpy pandas scikit-learn matplotlib 
Run Jupyter Notebook:
jupyter notebook 
What I Learned
Applying machine learning to genomic (SNP) data
Using Random Forest for prediction and feature importance
Evaluating models using R² score
Interpreting model outputs and validating results
Understanding the effect of noise on model performance
Author
Fatima Niknam
