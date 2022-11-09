# American-Express---Default-Prediction
Competitions from the kaggle platform: https://www.kaggle.com/competitions/amex-default-prediction

**Build**
```bash
$ git clone https://github.com/zeio99/American-Express---Default-Prediction.git
$ cd code
```

# 1. Steps to run
- 1 Download the raw dataset and save it to the input/amex-default-prediction directory.
Download the processed dataset to the input/amex-data-integer-dtypes-parquet-format directory
(https://www.kaggle.com/datasets/raddar/amex-data-integer-dtypes-parquet-format)
- 2 Run code/fe_process.py, the main purpose of this step is to generate the feature file, which takes some time to run
- 3 Run code/lgb.py, this code trains lgb
- 4 Run code/xgb.py, this code trains xgb (using GPU)
- 5 Run code/lgb_2.ipynb, which trains the second lgb
- 6 Run code/infer.ipynb to get the fusion results


# 2. Prerequisites
- pandas
- numpy
- lightgbm
- pyarrow
- pickle
- tdqm
