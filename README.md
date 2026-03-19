# Toxic Compound Prediction

This project performs Exploratory Data Analysis and builds a Random Forest model to predict whether chemical compounds are Toxic or NonToxic.

## Steps Performed
- Exploratory Data Analysis (EDA)
- Data preprocessing
- Feature selection
- Random Forest model training
- Cross-validation evaluation

## Tools Used
- Python
- Pandas
- Scikit-learn
- Seaborn
- Matplotlib
## Discussion On HyperParameter Tunin
## Hyperparameters Tuned

1.n_estimators

Number of trees in the forest

More trees → better performance but slower

2.max_depth

Maximum depth of each tree

Prevents overfitting

3.min_samples_split

Minimum samples required to split a node

Controls model complexity

4.min_samples_leaf

Minimum samples in a leaf node

Helps smooth predictions

## Observations

Grid Search explores all combinations → more accurate but slower

Random Search explores random combinations → faster, often close results

Tuned model usually:

Improves F1-score (important for toxicity classification)

Balances precision & recall

##Conclusion

After tuning hyperparameters using Grid Search and Random Search, the model performance improved compared to the default Random Forest model. Grid Search produced slightly better results but required more computation time, while Random Search provided a faster alternative with competitive performance.
