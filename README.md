# Chicago_car_crashes_project
<div align="center">
  <img src="https://github.com/JIMWAMAE/Chicago_car_crashes_project/blob/main/images/Chicago.jpg?raw=true" alt="Chicago">
</div>
Author- Jimcollins wamae
## Overview

Our objective was to develop inferential classification models for the Vehicle Safety Board of Chicago using cleaned and formatted data on crashes, vehicles, and individuals involved in accidents from 2016 to 2020. Our goal was to categorize the primary contributory causes of car accidents into two groups: avoidable and unnavoidable.

## Business Understanding

The Vehicle Safety Board of Chicago has entrusted us with the task of conducting a comprehensive analysis of car crash data to enhance their understanding of the causes and factors influencing avoidable and unavoidable accidents in the region. Our project aims to delve deep into the available data, spanning from 2016 to 2020, to identify the primary contributory causes of crashes and uncover valuable insights that can drive actionable recommendations.

By leveraging advanced data analysis techniques and employing various classification models, our objective is to decipher the underlying patterns, correlations, and trends within the crash data. This analysis will enable us to differentiate between avoidable and unavoidable accidents, shedding light on the key factors that contribute to each category.

Through this project, we seek to address the following crucial business questions: What are the primary causes of avoidable accidents in Chicago? Which age groups are more susceptible to being involved in avoidable crashes? Are there specific road conditions or locations that pose a higher risk for avoidable accidents?

By gaining a deeper understanding of the factors influencing avoidable accidents, we aim to provide strategic recommendations that will assist the Vehicle Safety Board in formulating effective interventions and policies. These recommendations may include targeted driver education campaigns, infrastructure improvements in high-risk areas, or other measures aimed at reducing the occurrence of avoidable accidents and promoting overall road safety.

Ultimately, our project endeavors to contribute to the mission of the Vehicle Safety Board by providing data-driven insights and actionable recommendations. By equipping the Board with a comprehensive understanding of the causes and factors associated with avoidable accidents, we can collectively work towards creating a safer driving environment for the residents of Chicago and reducing the human and economic toll of car crashes in the region.
## Data Understanding

The Vehicle Safety Board would like to better understand the causes of crashes in the Chicago area. That way, they can focus their campaign on potentially preventing some of those crashes in the future. We used data from the City of Chicago Data Portal, which contains information about Chicago Car Crashes from January 2016 to December 2020. The target variable was “primary contributory cause” as recorded by the police officer at the scene of the crash. Some of our inferential variables “defect road”, “bad road conditions”, and “obscured vision” will help us in our analysis to see if a crash was preventable. 

## Data Preparation

We combined 3 different datasets that we found on the City of Chicago website. Those datasets were crashes, people, and vehicles. 

We conducted thorough data preparation on the provided datasets from the City of Chicago, which included vehicles, people, and crashes data. Our goal was to clean, transform, and integrate the data to ensure its quality and suitability for analysis. By addressing missing values, inconsistencies, we enhanced the reliability and accuracy of the data. Through feature engineering and data integration, we created new variables and established meaningful relationships between the datasets. The data preparation process forms the foundation for our subsequent analysis and modeling, enabling us to derive valuable insights and make informed recommendations to the Vehicle Safety Board of Chicago.

## Modeling

Our target had a distribution of .75 to .25. The 2 categories in the target are 1 for preventable and 0 for not preventable. Because our class balance was 2:1 , we did not SMOTE the minority class.

We modeled the data through iterative modeling. We used a decision tree model as our first simple model.  
We graded this model on accuracy score and it resulted in 0.72. This was our lowest score. Therefore we used this as our baseline. It was something simple and understandable yet still decent and something we could build on. 
We also graded this model on precision and got a result of 0.71.

our second model was the gradient boosting model which improved on the accuracy from our baseline model from 72% to 74%

we still worked to improve our model perfomance using the Adaptive boosting classifier which increased the accuracy as well though by a small margin 74.2% - 74.3%.

we further used other three models wich will be shown in the classification metrics table below.


In conclusion, the objective of the project was to identify the causes of accidents in Chicago in order to help reduce them. The target variable was categorized into two classes: avoidable and unavoidable accidents. After evaluating multiple machine learning models, the Random Forest algorithm emerged as the best model for this task.


## Evaluation

The Random Forest model achieved the following classification metrics:

Precision: 0.7663
Recall: 0.9021
Accuracy: 0.7580
F1 Score: 0.8287

These metrics indicate that the model performed well in predicting both avoidable and unavoidable accidents. The high precision suggests that the model had a low rate of false positives, accurately identifying avoidable accidents. The high recall indicates that the model had a low rate of false negatives, successfully capturing a large portion of actual avoidable accidents. The accuracy score reflects the overall correctness of the model's predictions, while the F1 score balances precision and recall.

Based on accuracy we can view the overal model perfomance compared to previous models. 


These results suggest that the random forest model can effectively identify the causes of accidents in Chicago, making it a valuable tool for reducing accidents by targeting specific risk factors. It provides a reliable framework for identifying avoidable and unavoidable accidents, enabling policymakers and relevant stakeholders to allocate resources and implement targeted interventions to mitigate the identified causes.

By leveraging the insights gained from the Random Forest model, it is possible to identify the key factors contributing to accidents in Chicago. This information can be used to implement targeted measures and interventions aimed at reducing the occurrence of accidents and improving road safety in the city.



## Conclusions

Based on our analysis, we have several recommendations to Vehicle Safety Board of Chicago to improve road safety and reduce preventable crashes in the Chicago area.

1. Fix damaged or defective roads: We recommend prioritizing the repair of roads in hot spot areas that have a higher frequency of non-preventable crashes. By addressing infrastructure issues, such as potholes or inadequate signage, we can create safer road conditions and minimize the occurrence of such incidents.

2. Invest in an online driver and behavior education campaign: Implementing an online driver education program can have a significant impact on reducing preventable crashes. This approach is not only affordable but also easily accessible to a wide audience. By providing educational resources and promoting safe driving practices, we can enhance driver awareness and decision-making skills.

3. Target the younger audience (age 20-39): Our analysis indicates that drivers within the age range of 20-39 accounted for a significant proportion of preventable crashes. Therefore, we recommend tailoring the driver education campaign to specifically target this demographic. By focusing on this age group, we can effectively address their unique driving behaviors and contribute to a substantial reduction in preventable accidents.

4. Cost-effectiveness of driver education: It is worth noting that investing in driver education yields multiple benefits. Not only is it a cost-effective solution compared to solely repairing damaged roads, but it also saves significant labor costs in the long run. By addressing driver behavior and improving road awareness, we can create a safer driving environment for all road users.

By implementing these recommendations, we believe we can make substantial progress in reducing preventable crashes in the Chicago area. It is crucial to allocate resources and collaborate with relevant stakeholders to ensure the successful implementation of these measures. Together, we can create a safer road environment and work towards the goal of minimizing accidents and their associated consequences.

## For More Information

See the full analysis in the [Jupyter Notebook](https://github.com/JIMWAMAE/Chicago_car_crashes_project/blob/main/index.ipynb) 

