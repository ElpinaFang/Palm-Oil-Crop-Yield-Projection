# Palm-Oil-Crop-Yield-Projection
A data-driven project to predict palm oil crop yields using machine learning techniques. Includes preprocessing, modeling, and evaluation steps for accurate agricultural forecasting.

Palm Oil (CPO) is one of the most widely produced and consumed vegetable oils globally. Indonesia, as a top producer and exporter, benefits from its economic value, use in cooking oil, and job creation. High rainfall, sunlight, and warm temperatures—like in Indonesia—are ideal for optimal production.
The objective to be achieved through big data analysis of agroclimatic data (temperature, humidity, land elevation, etc.) is to obtain the best machine learning model for predicting crop yield.

## Data
- Agroclimatic: NASA,   https://power.larc.nasa.gov/data-access-viewer/
- Crop Yield: FAOSTAT,   https://www.fao.org/faostat/en/#data/PP
- Granularitas: Annual
- Years: 1980 – 2020

### NASA

![image](https://github.com/user-attachments/assets/92a1b23e-76b9-4d3e-8376-41e093695395)


### Faostat

![image](https://github.com/user-attachments/assets/53bef5a7-2518-4817-9c6b-0f8bb9555b27)


## Pre-processing
- Data Aggregation
- Data Cleaning (Duplicate & Missing Value)
- Normalization
- Correlation Threshold = 0.2
- Training Split: 90:10

## Correlation

![image](https://github.com/user-attachments/assets/5b697054-bc4b-4b17-96e2-79522143deff)


## Machine Learning
- Decision Tree
- AdaBoost
- Extra Tree
- Random Forest
- GradientBoosting

## Result

![image](https://github.com/user-attachments/assets/434fb310-ea93-494b-895a-00250236b407)


## Data Augmentation – SMOTER-GN
- Synthetic Minority Over-Sampling Technique for Regression
- Conducts the Synthetic Minority Over-Sampling Technique for Regression (SMOTER) with traditional interpolation, as well as with the introduction of Gaussian Noise (SMOTER-GN)
- Selects between the two over-sampling techniques by the KNN distances underlying a given observation. If the distance is close enough, SMOTER is applied. If too far away, SMOTER-GN is applied.

## Correlation – After Augmentation

![image](https://github.com/user-attachments/assets/54986c7d-2100-4065-a950-93add9e762f3)


## Result After Data Augmentation

![image](https://github.com/user-attachments/assets/3cc0b715-4311-41e3-86a4-3d53ddb40d74)


## Decision Tree & Ada Boost

![image](https://github.com/user-attachments/assets/ba90fefa-1575-4c01-b947-09fec904bc6c)


## Extra Tree & Random Forest

![image](https://github.com/user-attachments/assets/5bd2fbc6-bd57-4428-9d41-664804b31bcc)


## Gradient Boost

![image](https://github.com/user-attachments/assets/e2a58ef2-0e1d-4cf8-9cd0-81b719c7d5e2)


## Summary
- Best MSE (Before Data Augmentation): Random Forest [0.004499]
- Best MSE (After Data Augmentation): Gradient Boosting [0.000395]
- The results of this experiment show that with data augmentation, we can achieve higher accuracy in several trained tree-based models.













 















