The patch contains the final codes and models files for the prediction of Air quality.

We are predicting 2 quantities here i.w Relative Humidity (RH) and Average Humidity (AH)
A technique called average ensemble learning is used to average the predicted values from two models for better performance

Explanation of the files:

1. regression_withXGBOOST.ipynb : This is the 1st model i.w XGBOOST model. The following video link will help you understand what XGBOOST is:
https://youtu.be/OtD8wVaFm6E  (Watch all the 4 parts if possible. Either way 1st and 2nd works)
2. ANN_Final_Build.ipynb : Thisis the 2nd model where artificial neural net or fully connected NN is used for the prediction
3. ensemble_final : this file helps us in making the dataframes for the average models and we apply average formula here.

4. AirQualityUCI.xls: This is the original Dataset
5. RGBoost_Implemented.csv: This is the file where predicted results from XGBOOST are added to the end i.e more 2 columns are added
6. NN_Implemented.csv: This is the file where predicted results from ANN are added to the end i.e more 2 columns are added

Now the training for the XGBOOST takes almost 15-20 minutes for 1 prediction and we have 2 predictions. Thats why XGBOOST trees are to be saved.

7. RH_XREG.json: Relative Humidity Prediction via XGBOOST model saved as json format (Similar to saving neural network weights)
8. AH_XREG.json: Average Humidity Prediction via XGBOOST model saved as json format (Similar to saving neural network weights)

