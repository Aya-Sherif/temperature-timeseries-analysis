# Temperature Forecasting

This project focuses on forecasting daily minimum temperatures using time series models. The main goal is to practice and demonstrate concepts learned in class, particularly around seasonal forecasting and error analysis.

## Models Used

- **Persistence Model**: A naive baseline where the next value is assumed to be equal to the current one.
- **SARIMA Model**: A seasonal ARIMA model capturing trend and yearly seasonality (SARIMAX(1,0,1)x(1,1,1,365)).

## Dataset

The dataset contains over 3,600 daily minimum temperature values. It was sourced from a public dataset, often used for time series modeling tasks.
you can find it here 👉 [Kaggle](https://www.kaggle.com/datasets/shenba/time-series-datasets/data?select=daily-minimum-temperatures-in-me.csv)

## Workflow Summary

1. Data cleaning and visualization
2. Fitting the Persistence and SARIMA models
3. Forecasting and evaluating accuracy
4. Comparing model performance using various metrics

## Accuracy Metrics Used

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)
- Symmetric MAPE (sMAPE)
- Median Absolute Percentage Error (MDAPE)
- Geometric Mean Relative Absolute Error (GMRAE)

## Results Summary

| Metric | Persistence | SARIMA |
|--------|-------------|--------|
| MAE    | 2.02        | 2.06   |
| RMSE   | 2.60        | 2.61   |
| MAPE   | 21.34%      | 22.63% |
| sMAPE  | 20.01%      | 19.81% |
| MDAPE  | 14.62%      | 14.82% |
| GMRAE  | 0.00        | 0.00   |

## Notes

- The SARIMA model took over 5 hours to run due to high seasonality (365-day cycle) and large dataset size.
- Multiple reruns were required due to system crashes, highlighting the importance of memory-efficient modeling.

## License

This project is for educational use.

