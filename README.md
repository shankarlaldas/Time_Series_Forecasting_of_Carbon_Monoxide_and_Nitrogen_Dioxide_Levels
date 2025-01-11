# Time Series Forecasting of Carbon Monoxide and Nitrogen Dioxide Levels
 <br/><br/>
## ⚠️ Warning Because of large file size. Please go to collab for code view
[Colab Link](https://colab.research.google.com/drive/10haMPRWySWOy8xc51LNglIa8TfgD9_Vp?usp=sharing)
<br/><br/>
## Summary

### Model Performance

- **CO₂ Prediction:**

  - **Model Used:** Random Forest Regression
  - **R² Score:** 0.8047
  - **Observation:** The model performs reasonably well in predicting CO₂ levels, capturing a significant portion of the variance in the data.

  - **Model Used:** LSTM
  - **Performance Metric:** RMSE
  - **RMSE Value:** 0.330203661711536
  - **Observation:** The LSTM model shows a relatively good fit for CO predictions, with the predicted values closely following the actual values. However, there are some deviations, particularly around the peaks.

- **NO₂ Prediction:** 
    -**Model Used:**: Random Forest Regression
    - **R² Score:** 0.8434
    - **Observation:** The model demonstrates strong performance in predicting NO₂ levels, explaining a substantial amount of the variance.

    - **Model Used:** LSTM
    - **Performance Metric:** RMSE
    - **RMSE Value:** 19.072198814483876
    - **Observation:** The LSTM model for NO2 predictions shows more significant deviations from the actual values, indicating a higher error rate compared to the CO model.

    
- **NO₂ Prediction Plot:**

  - The plot shows the actual vs. predicted NO₂ levels with confidence intervals.
  - The forecast starts from April 4, 2015, and extends to May 6, 2015.
  - The confidence intervals widen over time, indicating increasing uncertainty in the predictions.

- **CO₂ Prediction Plot:**
  - The plot shows the actual vs. predicted CO₂ levels with confidence intervals.
  - The forecast starts from April 4, 2015, and extends to May 6, 2015.
  - The confidence intervals also widen over time, reflecting the growing uncertainty in the predictions.

## Future Modifications

### Data Preprocessing

- **Normalization:** Ensure that the data is properly normalized to improve model performance.
- **Feature Engineering:** Consider adding more features that might influence CO and NO2 levels, such as weather conditions, traffic data, etc.

### Model Tuning

- **Hyperparameter Optimization:** Experiment with different hyperparameters such as the number of LSTM layers, number of units, learning rate, etc.
- **Regularization:** Implement techniques like dropout to prevent overfitting.

### Advanced Models

- **Ensemble Methods:** Combine predictions from multiple models to improve accuracy.
- **Hybrid Models:** Use a combination of LSTM and other models like CNN or GRU to capture different aspects of the data.

### Evaluation Metrics

- **Additional Metrics:** Besides RMSE, consider using other evaluation metrics like MAE (Mean Absolute Error), MAPE (Mean Absolute Percentage Error), and R-squared to get a more comprehensive understanding of model performance.

### Cross-Validation

- **K-Fold Cross-Validation:** Use k-fold cross-validation to ensure the model's robustness and generalizability.

### Real-Time Data

- **Incorporate Real-Time Data:** If possible, incorporate real-time data to continuously update and improve the model's predictions.

### Visualization

- **Improved Visualization:** Enhance the visualization of results to better understand the model's performance and areas of improvement.

By implementing these modifications, the accuracy and reliability of the predictions for both CO and NO2 can be significantly improved.


### Conclusion

The Random Forest Regression model shows promising results for predicting CO₂ and NO₂ levels. However, there is room for improvement through advanced feature engineering, hyperparameter tuning, ensemble methods, and time series considerations. By implementing these modifications, the model's performance and interpretability can be further enhanced.
