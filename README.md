# ML-based Circuit Delay Prediction for CMOS Timing Analysis

## Motivation
Accurate circuit delay estimation using SPICE simulations is computationally expensive.
This project explores machine learning models to predict CMOS inverter timing parameters
across voltage corners, enabling faster early-stage timing analysis.

## Problem Statement
Given circuit parameters such as capacitive load and supply voltage, predict:
- Rise Delay
- Fall Delay
- Average Delay (DAVG)

using supervised machine learning models.

## Approach
- Feature engineering on capacitive load and voltage parameters
- Baseline Linear Regression vs Gradient Boosting comparison
- Per-voltage-corner modeling
- 5-fold cross-validation for robustness
- Derived average delay (DAVG) from predicted rise/fall delays

## Results
- Gradient Boosting consistently outperformed Linear Regression
- Achieved strong R² scores with RMSE reduced by ~28% compared to linear regression
- Demonstrated feasibility of ML-based timing estimation

## Tech Stack
- Python  
- scikit-learn  
- pandas, numpy  
- matplotlib.
# Final Result Output:-
### Circuit Diagram:-
![Home](Circuit_Diagram.jpeg/Circuit Diagram.png)
### FinalResult:-
| Result3V | Result4V | Result 5V |
|-------|--------|--------|
| ![Result3V](Result3V/FinalResult.png) | ![Result4V](Result4V/FinalResult.png) |
