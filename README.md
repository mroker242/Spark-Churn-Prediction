# Spark-Churn-Prediction

Churn is one of the most important aspects of a business; that is, preventing churn. This project focuses on classifying
churn and making predictions based on that classification. The `Sparkify.ipynb` file contains the following:

- Cleaning
- Data Exploration
- Feature Engineering
- Data Modeling

## Dependencies

- SparkSession
- PySpark Functions: avg, col, concat, count, desc, explode, lit, udf, split, to_date, from_unixtime, unix_timestamp
- PySpark Types: IntegerType, StringType
- pyspark Classification: LogisticRegression, DecisionTreeClassifier
- PySpark Features: VectorAssembler
- PySpark Tuning: CrossValidator, ParamGridBuilder, TrainValidationSplit
- matplotlib

## File Descriptions

- Sparkify.ipynb
- mini_sparkify_event_data.json
- https://medium.com/@mroker/will-your-customers-leave-d38fa8ca4fa


## Resources

- https://towardsdatascience.com/build-an-end-to-end-machine-learning-model-with-mllib-in-pyspark-4917bdf289c5
- https://spark.apache.org/docs/latest/ml-pipeline.html
- https://towardsdatascience.com/feature-engineering-for-machine-learning-3a5e293a5114

## Analysis & Results

For this project, we have had to classify users who have churned. Not only have we had to classify these users but we had to build a model that would make predictions.

The approach taken to this problem was to firstly define what churn is. This was defined by using the event of Cancellation Confirmation. If the user cancelled their service, they were defined as churn.

After defining churn, some features were extracted such as gender and level. These features were used and a model was trained and it was used to make predictions. The accuracy score of the using the Logistic Regression training model was 58%.

Overall, this score was ok, but could be improved. This could possibly be done by extracting more features.