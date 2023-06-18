# Capstone-3-Daegu-Apartment

**Context:**
Apartments are one of the answers to the housing needs of modern society due to limited residential land and dense business activities in urban areas. Therefore, it will be very interesting to examine apartment prices influenced by various internal and external factors. 

Individuals or companies usually make apartment (unit) offers. Bidders can sell units on a platform by determining their apartments’ prices. That way is quite difficult for apartment owners to adjust to market prices. If the price is too high compared to the market price, it will certainly be difficult to make sales. Conversely, if it is too low, the owner will find it difficult to get maximum profit.

**Problem Statement:**
Apartments are one of the answers to the housing needs of modern society due to limited residential land and dense business activities in urban areas. Therefore, it will be very interesting to examine apartment prices influenced by various internal and external factors. 

Individuals or companies usually make apartment (unit) offers. Bidders can sell units on a platform by determining their apartments’ prices. That way is quite difficult for apartment owners to adjust to market prices. If the price is too high compared to the market price, it will certainly be difficult to make sales. Conversely, if it is too low, the owner will find it difficult to get maximum profit.

**Conclusion:**
- Based on the modeling that has been done, the features HallwayType_Terraced, YearBuilt, and Size(sqf) are the most influential features on SalePrice. However, it does not mean that other features do not have an impact on the target variable.

- The evaluation metric used for the model is MAE (Mean Absolute Error). Looking at the MAE value produced by the model after hyperparameter tuning using XGBoost, which is 38515.607468, we can conclude that if this model is used to estimate apartment prices in Daegu within the range of values it was trained on (maximum price of USD 585840), the estimated error, as indicated by MAE, is relatively small at 6.5%. However, when compared to the model trained on a minimum price of USD 40,088, the error is significantly large.

- However because MAE represents the average prediction error in the same unit as the target variable, which is the apartment price, So, we cannot simply calculate the predicted price by adding or subtracting the MAE value only from the Sale Price. The prediction of the price involves considering the calculated features and their impact based on the XGBoost model.

- In order to predict the price accurately, we **need to utilize the trained XGBoost model along with the relevant features**. **The model takes into account the importance and influence of each feature on the predicted price**. **By inputting the appropriate feature values into the model, we can obtain a more reliable and accurate prediction of the price**.

- Overall, using the XGBoost model that has undergone the tuning process as the most accurate model for predicting apartment prices in Daegu. This model can provide price estimations with a lower level of error, making it a more reliable tool in supporting business decisions related to determining apartment prices. By relying on this tuned XGBoost model, businesses can make more accurate price estimations and optimize pricing strategies. Due to the efficient and flexible nature of the XGBoost algorithm, property agents in Daegu can predict apartment prices and earn substantial commissions from seller and they can also answer to potential buyer about apartement price with the prediction.

- **Recomendations:**
Recommendations for Business are:

- Agent property sales / marketing can use this model for baseline price that depends on the feature in this model. [['Daegu Apartement Price Prediction']](https://rgt88-capstone-3-daegu-apartment-app-caps-4m6wr1.streamlit.app/)

Recommendations for improving the modeling are:

- Add additional features or facilities that can potentially influence the SalePrice, such as the longtitude and latitude to know and plot the area.
- Explore more complex algorithms that can potentially minimize errors deep learning models (e.g., neural networks).

By implementing these recommendations, you can potentially improve the performance of the model and make more accurate predictions for apartment prices in Daegu.
