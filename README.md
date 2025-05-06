# Machine Learning 1

Team Members:
- Cezary Kuźmowicz
- Wojciech Hrycenko

## Assessment rules
### General information
In teams of at most 2 persons students will work on two practical machine learning projects – one for regression and one for classification. Please inform the lecturer about the team members by email pwojcik@wne.uw.edu.pl or sm.lis@student.uw.edu.pl the latest by midnight 2025-04-18.

## Datasets
The data is exactly the same for all teams.

## Appartments for regression
Your task is to apply various ML algorithms (see the rules below) to build a model explaining the prices of appartments based on the training sample and generate predictions for all observations from the test sample.

The dataset consists of apartment records with the following features:

unit_id – Unique (and anonymized) identifier for each apartment.

obj_type – Type of apartment or object (categorical, anonymized).

dim_m2 – Apartment size in square meters.

n_rooms – Number of rooms.

floor_no – The floor on which the apartment is located.

floor_max – Total number of floors in the building.

year_built – The year the building was constructed.

dist_centre – Distance from the apartment to the city center.

n_poi – Number of points of interest nearby.

dist_sch – Distance to the nearest school.

dist_clinic – Distance to the nearest clinic.

dist_post – Distance to the nearest post office.

dist_kind – Distance to the nearest kindergarten.

dist_rest – Distance to the nearest restaurant.

dist_uni – Distance to the nearest college or university.

dist_pharma – Distance to the nearest pharmacy.

own_type – Ownership type (categorical, anonymized).

build_mat – Building material (categorical, anonymized).

cond_class – Condition or quality class of the apartment (categorical, anonymized).

has_park – Whether the apartment has a parking space (boolean).

has_balcony – Whether the apartment has a balcony (boolean).

has_lift – Whether the apartment building has an elevator (boolean).

has_sec – Whether the apartment has security features (boolean).

has_store – Whether the apartment has a storage room (boolean).

price_z – Target variable: Apartment price (in appropriate monetary units) to be predicted – only in the training sample

src_month – Source month (time attribute).

loc_code – Anonymized location code of the apartment.

market_volatility – Simulated market fluctuation affecting the apartment price.

infrastructure_quality – Indicator of the building’s infrastructure quality, partially based on the building’s age.

neighborhood_crime_rate – Random index simulating local crime rate.

popularity_index – Randomly generated measure of the apartment’s attractiveness.

green_space_ratio – Proxy variable representing the amount of nearby green space, inversely related to the distance from the city center.

estimated_maintenance_cost – Estimated cost of maintaining the apartment, based on its size.

global_economic_index – Simulated economic index with minor fluctuations across entries, reflecting broader market conditions.

### Files Provided
appartments_train.csv – training data contains 156454 observations and 34 columns along with the target variable price_z.

appartments_test.csv – test data contains 39114 observations and 33 columns without the target variable.

## Insurance for classification
Your task is to apply various ML algorithms (see the rules below) to build a model explaining travel insurance claim outcomes based on the training sample and generate predictions for all observations from the test sample.

The dataset includes travel insurance policy records with the following columns:

reward – Commission value earned on the insurance sale

claim_status – Target variable (0 = Not Approved, 1 = Approved) Only in training sample

person_gender – Gender identifier of the insured person

entity_type – Type of selling entity

channel – Distribution channel used

support_interactions – Number of customer service interactions

agent_id – Identifier for the selling agent

customer_score – Computed value between 0-1 based on customer metrics

entity_a – Identifier of the agency that sold the policy

person_age – Age of the insured person

location – Destination of the trip

revenue – Net sales value of the policy (when <0 it covers discounts)

product_id – Name of the insurance product

trip_length – Duration of the insured trip in days

### Files Provided
insurance_train.csv – training data contains 56993 observations and 14 columns along with the target variable claim_status

insurance_test.csv – test data contains 6333 observations and 13 columns without the target variable

## Requirements
### Exploratory Data Analysis:
– Analyze the dataset to identify key patterns, correlations, and potential challenges introduced by the additional variables. – Visualize distributions and relationships among variables.
### Feature Engineering:
– Consider transformation or scaling of variables as needed. – Evaluate the impact of the supplementary variables on model performance.
### Modeling:
– Build, train, and compare multiple regression models. – Optimize model hyperparameters using cross-validation.
### Predictions:
– Generate predictions for all observations in the test dataset. – Document model performance and reasoning behind the selected approach.
### Documentation:
– Provide a clear explanation of your analysis, modeling choices, and any challenges faced while integrating the additional variables.
## Various algorithms
For each of the datasets please consider and compare at least 3 different ML algorithms discussed in the ML1 course (e.g. linear/logistic regression, KNN, LASSO, ridge, elastic net, SVM/SVR with various kernel functions). You can also apply in addition any other algorithms you know, but they cannot be used instead of the ones mentioned before.

## Selection of the best algorithm
The choice of the final algorithm applied to generate predictions should be clearly explained in the presentation.

HINT !!!!! Use the internal division of the training data into train/validation/test samples to make sure that you correcly assess the performance of your models on the new data.

## Performance measure
The performance of predictions will be based on:

RMSE for the appartments dataset
balanced accuracy for the insurance dataset
Please report the expected value of a particular performance measure (expectation for the test sample) in your presentation.

## Points
In total 60 points can be collected – 30 for each project:

### Presentation in class
Its structure, way of presenting, etc. (10 pts for each project)
### Presentation contents
Assessed by the lecturer after you present in class (10 pts for each project)
### Out of sample performance (10 pts for each project):
- 10 if predictive performance in top quartile group (best),
- 7.5 if predictive performance in the 2nd quartile group (good),
- 5 if predictive performance in the 3rd quartile group (below average),
- 2.5 if predictive performance in the 4th quartile group (unlucky),

## Presentations
The presentation together with the full codes have to be submitted by email to the lecturer pwojcik@wne.uw.edu.pl or sm.lis@student.uw.edu.pl until midnight eod 2025-05-31. The codes should load the training data, train the single best algorithm, apply this model on the test data and save test data predictions in the csv file, which should be also attached. The file with predictions should only include the observation id and the predicted value of the outcome variable.

Do NOT include all the codes which you applied to find the best algorithm, parameter search, etc. ONLY a simple code for a FINALLY selected algorithm i.e. with the selected set of best performing parameters for each dataset.

All teams will give presentations (not more than 10 minutes) informing about the algorithms considered, selection process and their expected results.

Presentations will take place on 2025-06-02 for groups taught by Piotr Wójcik and on 2025-06-04 for groups taught by Szymon Lis and Michał Woźniak.

Groups that do NOT present their results in class will not be graded.

## Important dates again
- 2025-04-18 by end of day – submission of information about the team members
- 2025-05-31 by 23:59 – submission of presentations, codes and test sample predictions,
- 2025-06-02 or 2025-06-04 – in class presentations – depending on the group.
Each submission should be done via email to pwojcik@wne.uw.edu.pl or sm.lis@student.uw.edu.pl before midnight of the deadline day if not stated otherwise.
