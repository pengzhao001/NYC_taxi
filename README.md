This submission includes the following 3 files:

1. A jupyter notebook (Python 3 kernel) containing all the codes, analysis, and visualizations.
2. A pdf report which was converted from the jupyter notebook. They have the same content although the jupyter notebook has a better layout in the browser. 
3. A pickle file of the optimized XGBoost regression model (xgb_opt.pkl).


Instruction manual:

1. This work was done in Python 3 with several packages, including Pandas, Scikit-learn, statsmodels, geopy, xgboost, pickle, seaborn. Please install these packages by pip install xxxx before executing the code blocks.
2. Please put the data file and the jupyter notebook in the same directory.
3. The hyperparameter tuning procedure for the XGBoost regression model took more than 10 hours on my laptop (macOS 10.14.1, 2.7 GHz i7, 16 GB LPDDR3 Memory, Radeon Pro 455 2G GPU). Please skip this part if you want to do a quick test of the codes.
4. Please use the following way to load the pickled model.

import pickle
with open("xgb_opt.pkl", "rb") as f:
    loaded_model = pickle.load(f)
