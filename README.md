# Handson-L10-Spark-Streaming-MachineLearning-MLlib

**Environment Setup**
Run These Commands below
1. pip install pyspark
2. pip install faker
3. pip install numpy
4. sdk install java 17.0.10-tem #when prompted select this as default


**Task 4**<br>
Within Task 4 I was required to finish the Machine Learning module. This included loading training data, casting types to Double for ML. I then had to go through and create VectorAssembler to combine feature columns into single features vector. I then created a LinearRegression model instance and then trained the model by fitting it to the training data given. I saved the model and then moved it over to the models folder. Once I simulated the streaming with Faker I then had to go through and load the model we pre-trained, use the VectorAssembler to transform the distance_km column of streaming data into features vector. use loaded model to make predictions and calculate the standard deviation with the fare_amount and then the prediction from the model. Some of the results seemed pretty far off however I really believe this was implemented correctly.<br>

Task4py Screenshot
![Terminal Output T6](image.png)

**Task 5**<br>
Similarly to Task 4 I had to import the proper libraries from pyspark.ml, then I aggregated data into 5-minute time windows and calculated the average fare. I then added two new columns "hour_of_day & minute_of_hour into a new variable hist_features that contained 
![Terminal Output T5](image-1.png)