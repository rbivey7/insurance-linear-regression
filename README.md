# insurance-linear-regression

Determining the financial impact of age and smoking on insurance premiums.

Medical Insurance Cost Analysis 
<img width="902" height="577" alt="Screenshot 2026-01-16 at 5 18 19 PM" src="https://github.com/user-attachments/assets/8c4c6793-68d8-4ef6-a37b-9de144776a7a" />

Project Overview

This project uses Python and Linear Regression to analyze how age and lifestyle choices (specifically smoking) affect medical insurance costs.The goal was to determine if we could accurately predict insurance charges based on age alone, and to quantify the financial penalty associated with smoking.

Key Findings

The "Hidden" Smoker Group: Initial analysis yielded a weak correlation ($R^2 \approx 0.39$). Further investigation revealed that smokers and non-smokers form two distinct cost clusters.Data 

Cleaning Discovery: The dataset contained inconsistent formatting in the smoker column (hidden whitespace), which required cleaning to correctly segment the data.

Age is a Strong Predictor: Once smokers were removed and the data was cleaned, age became a highly accurate predictor of cost for the remaining population ($R^2 \approx 0.87$).

The Smoker Penalty: Smoking adds a massive flat fee to insurance costs (approx. $23,000), regardless of age.

Technologies Used

Python 3Pandas: For data manipulation and cleaning (fixing the whitespace bug).
Matplotlib: For visualizing the "Smoker vs. Non-Smoker" cost gap.
Scipy (Stats): For calculating the Slope, Intercept, and R-Squared values.

Visual Analysis

Initial Approach: Running regression on the entire dataset showed a noisy, unreliable model.
Segmented Approach: Splitting the data revealed that non-smokers follow a strict linear path, while smokers pay a premium that skews the average.

How to Run This Project

Clone the repository:Bashgit clone https://github.com/rbivey7/insurance-linear-regression.git
Install the required packages:Bashpip install pandas matplotlib scipy
Open the Jupyter Notebook:Bashjupyter notebook insurance_costs.ipynb

Author Robert Ivey
[LinkedIn Profile](https://www.linkedin.com/in/robert-ivey-50892b12a/)
[GitHub Profile](https://github.com/rbivey7)
