# ML_BigMart-Sales-Prediction-Project
The goal is to build a regression model that can predict the sales of each product (Item_Outlet_Sales) in a particular store based on the available product and outlet information. Accurate prediction of product sales is critical for effective supply chain management, store planning, and promotional strategies.

**Project Workflow:**

To solve the BigMart Sales Prediction problem, a comprehensive machine learning pipeline was developed that integrates data analysis, preprocessing, feature engineering, and regression modeling into a coherent workflow.

The process began with exploratory data analysis (EDA) to understand the underlying patterns and statistical properties of the data. This stage involved examining the distributions of features, identifying missing values, and assessing potential outliers. These insights were used to inform the data cleaning and transformation steps that followed.

Unlike workflows where the test data is preprocessed separately, this project handled both the training and test datasets together within a single notebook. This approach was chosen to maintain consistency in preprocessing operations, especially during the ordinal encoding of categorical variables. It ensured that both datasets were encoded using the same mapping, avoiding any discrepancies during prediction.

Feature engineering techniques were employed to extract additional insights from the raw data. This included transforming variables or deriving new ones that could provide the model with a more informative representation of the input space. Subsequently, feature scaling was applied to the independent variables to normalize their distributions and optimize model performance.

Multiple regression models were tested during the modeling phase. Despite the advanced capabilities of models like XGBoost, the Random Forest Regressor, and LGBoost Regressor consistently delivered better results on the validation set. This model was selected as the final predictive model due to its superior performance with the given data characteristics.

After training, predictions were generated for the test set using the LGBoost Regressor model. The predictions were already in their original scale and were exported directly to a CSV file.
