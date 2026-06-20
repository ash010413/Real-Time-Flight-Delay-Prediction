# Real-Time Flight Delay Prediction

This was my final machine learning project in 2023. It grew out of the Python
and machine learning coursework now collected in
[ML Foundations](https://github.com/ash010413/ml-foundations).

The project combines US flight records and weather observations from 2016 and
2017 for 15 airports. It uses a two-stage approach:

1. classify whether a flight will arrive at least 15 minutes late; and
2. estimate the delay duration for flights classified as delayed.

The notebooks cover data cleaning and merging, categorical encoding, class
imbalance, random under-sampling, random over-sampling, SMOTE, model comparison,
and regression. The accompanying report compares Logistic Regression, Decision
Trees, Random Forest, Extra Trees, and XGBoost. In the recorded results, XGBoost
was the best-performing delay-duration regressor.

## Files

- `flight-delay-prediction.ipynb` contains the analysis and modelling.
- `flight-delay-project-report.pdf` is the 13-page project report.

## Running it

The source datasets are not included. The notebook expects these files under a
`data` directory:

```text
data/flight-data.csv
data/weather-data.csv
```

After supplying compatible data, install Jupyter, pandas, scikit-learn,
imbalanced-learn, XGBoost, and the plotting libraries imported by the notebooks.
The code was written in 2023, so current package versions may require changes.

## Status

Archived academic project. Despite the original title, this repository contains
the modelling work and report rather than a deployed real-time prediction
service.
