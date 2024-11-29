# Design and Evaluation of a Longitudinal Survey of Subjective Emotional States, Events and Sleep Quaility Metrics
## Aim:
This project will investigate the relationship between well-being factors and sleep quality. Main focus will be on the predictive abilities of these factors. Descriptive analysis will be carried out to determine patterns as well.
## Hypothesis:
Well-being factors are suitable predictors of sleep quality.
## Data:
For each day, around 10 features will be recorded on a survey. 7 of 12 features are continous variables, which describe the emotional states (ES) as follows.
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
A mini web application will be implemented via Python's *flet* library to collect data. An SQL database will be employed to collect analysis-ready data. A single widget will be implemented with input boxes for continous features and dropdown menu for binary ones. SQL data will be read, processed and analyzed with Python's *pandas* and *scikit-learn* libraries. By the end of the project's deadline, the data from the Health application will be recorded on an Excel file. Both data will be merged and analyzed.
## Method:
###
