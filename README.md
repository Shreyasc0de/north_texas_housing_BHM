# Bayesian Hierarchical Modeling: North Texas Housing Trends
### An Application of Probabilistic Programming & Explainable AI

## 📌 Project Overview
This project leverages **PyMC** to build a varying-intercept hierarchical model. 
As an MS student in **Applied Statistics and Data Analytics (ASDA)**, I developed this 
to demonstrate how partial pooling can recover "ground truth" parameters in nested 
datasets—specifically looking at how geography (County-level) influences housing 
prices in North Texas.

## 🏗️ The Model Architecture
We define a hierarchical structure where each county is a level-2 intercept:
- **Level 1 (Global):** The North Texas baseline.
- **Level 2 (County):** Dallas, Tarrant, Collin, and Denton offsets.
- **Level 3 (Observation):** Individual property square footage.

## 🧪 Technical Highlights
- **Inference:** MCMC sampling with the NUTS (No-U-Turn Sampler).
- **Diagnostics:** Verified convergence with $\hat{R}$ metrics and trace visualizations.
- **XAI focus:** Unlike black-box regression, this model provides full posterior 
distributions for every parameter, ensuring trust and transparency.

## 🛠️ Tools Used
`Python` `PyMC` `ArviZ` `Pandas` `NumPy`
