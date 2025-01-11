# Design and Evaluation of a Longitudinal Survey of Subjective Emotional States, Events and Sleep Quaility Metrics
## Aim:
This project will investigate the relationship between well-being factors and sleep quality. Main focus will be on the predictive abilities of these factors. Descriptive analytics will be applied to determine patterns as well.
## Hypothesis:
Well-being factors are suitable predictors of sleep quality and there exists patterns among interactions between emotional states of an individual.
## Data:
For each day, around 10 features will be recorded on a survey. 7 of 10 features are continous variables, which describe the emotional states (ES) as follows.
* Anger
* Anxiety
* Awareness
* Fear
* Joy
* Mindfulness
* Motivation

*The scoring will be based on a scale between 1 to 10.*

Rest of the features are the answers to (Yes/No) questions that describe emotional events (EE).
* Did you experience any striking events that had substantial effect?
* Did you boost your mindfulness with a technique such as yoga, meditation, prayer etc.?
* Did you have a social interaction, spontaneous or planned?

Main target features will be collected from an iPhone's Health application geared with an Apple Watch.
* Time in Bed
* Time in REM

*The ratio of the two also will be calculated programmatically as the feature of interest.*

| Date | ES1 | ES2 | ES3 | ES4 | ES5 | ES6 | ES7 | EE1 | EE2 |  EE3 | time_in_bed | time_in_rem | ratio | 
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | 
| 01.11.2024 | 10  | 10  | 10  | 10  | 10  | 10  | 10  | Yes | Yes | Yes | 8  | 2 | 0.25 |

*An example of an instance is given above.*

## Data Collection:
A mini web application will be implemented via Python's *flet* library to collect data. An SQL database will be employed to collect analysis-ready data. A single widget will be implemented with input boxes for continous features and dropdown menu for binary ones.

The application live on the following link: https://ihappy-bold-haze-9843.fly.dev/

** Demo User:**
username: *demo*
password: *demo*

SQL data will be read, processed and analyzed with Python's *pandas*, *scikit-learn* and *scipy* libraries. *matplotlib* and *seaborn* libraries are used for data visualization.

Historical data is exported from **iOS Health** application and stored on the SQL as a table where each instance is described by 3 features: 
* date
* time in bed
* time in REM
 
## Method:
### 1) Exploratory Data Analysis
* Mean and Standard Deviation
* Histogram
* Violin Plot
* Correlation
* Principal Component Analysis
* Hypothesis Testing - Chi Square

### 2) Predictive Data Analysis
* Linkage Tree and Dendrogram
* KMeans
* Regression
* Decision Trees
* XGBoost
* SVM

## Analysis, Results & Discussion:
[Report][1]

[1]: https://github.com/ecembalikk/dsa210-proj/blob/main/analyze.ipynb "Analysis and Report Notebook"
