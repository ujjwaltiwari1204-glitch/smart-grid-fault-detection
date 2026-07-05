# Smart Grid Fault Detection using Machine Learning

## Overview
A machine learning project that automatically detects electrical faults in power distribution networks using voltage and current measurements from three-phase power systems.

## Problem Statement
Electrical faults in power grids can cause equipment damage, power outages, and safety hazards. Manual fault detection is slow and unreliable. This project builds an ML model that detects faults automatically with 99.79% accuracy.

## Dataset
- **Source:** Kaggle — Electrical Fault Detection and Classification (esathyaprakash)
- **Size:** 12,001 samples, 6 features
- **Features:** Three-phase current measurements (Ia, Ib, Ic) and voltage measurements (Va, Vb, Vc)
- **Target:** Binary classification — Fault (1) or No Fault (0)
- **Class distribution:** 6505 no-fault, 5496 fault (nearly balanced)

## Approach
1. Loaded and explored the dataset (EDA)
2. Checked for missing values and class balance
3. Visualized voltage waveforms for all three phases
4. Trained a Random Forest Classifier (100 trees)
5. Evaluated model performance on unseen test data
6. Analyzed feature importance to understand which measurements matter most

## Results
| Metric | Score |
|--------|-------|
| Accuracy | 99.79% |
| Precision | 1.00 |
| Recall | 1.00 |
| F1-Score | 1.00 |

## Key Finding
Current measurements (Ia, Ib) are the most important features (68% combined importance), which aligns with electrical theory — faults cause dramatic current spikes while voltage changes are more gradual.

## Technologies Used
- Python
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab
- GitHub

## Project Structure
