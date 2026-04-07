🧬 Genomic Prediction using SNP Data and Machine Learning
📌 Overview
This project demonstrates how machine learning can be applied to genomic data to predict a quantitative trait and identify important genetic markers (SNPs).
A simulated dataset is used to mimic real-world genomic selection scenarios.
🎯 Objectives
Simulate SNP genotype data (encoded as 0, 1, 2)
Generate a quantitative trait influenced by selected SNPs
Train a machine learning model (Random Forest)
Evaluate model performance using R² score
Identify important SNPs using feature importance
Compare predicted SNPs with true causal SNPs
⚙️ Methodology
Data Simulation
Generated 500 samples with 300 SNPs
Selected a subset of SNPs as true causal variants
Added controlled noise to simulate realistic conditions
Model Training
Used RandomForestRegressor
Split data into training and testing sets (80/20)
Evaluation
Performance measured using R² score
Feature Importance
Extracted SNP importance from the trained model
Validation
Compared top predicted SNPs with true SNPs
📊 Results
Model: Random Forest Regressor
R² Score: ~0.63
✅ Successfully identified 100% of true SNPs
🧠 Key Insight
The model effectively captured the underlying signal in the simulated dataset and was able to perfectly recover all causal SNPs.
This highlights the power of machine learning in genomic prediction tasks.
📈 Example Output
Top important SNPs visualized using bar plots
Comparison between true and predicted SNPs
🛠️ Technologies Used
Python
NumPy
Pandas
Scikit-learn
Matplotlib
▶️ How to Run
Install dependencies:
pip install numpy pandas scikit-learn matplotlib 
Run Jupyter Notebook:
jupyter notebook
Author
Fatemeh Niknam
Notes
This project is based on simulated data, so results may differ from real genomic dataset with more complex genetic architectures.