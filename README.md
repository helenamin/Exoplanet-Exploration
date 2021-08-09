# Exoplanet-Exploration

![planets View](images/exoplanets.jpg)

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Introduction](#Introduction)
- [Structure](#Structure)
- [Setup](#Setup)
- [Analysis](#Analysis)
- [Contributors](#Contributors)
- [Technology](#Technology)

## Introduction

The NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets
outside of our solar system. This data collected for over nine years of period is being used to process and
predict scores. 


## Structure
```
 
Exoplanet-Exploration
|
|__data/                            # Directory for the data files
|     |__ exoplanet_data.csv
|
|__ images/
|     |__ exoplanets.jpg
|     |__ pythonlogo.png
|
|__ model_1.ipynb              # Data Modeling jupyter notebook file
|__ gitignore file
|__ README.md                       # read me file
                   

```

## Setup

Initially, the raw dataset was preprocessed and removed unnecessary columns and dropped null value
rows. Then the data was scaled using MinMaxScaler followed by splitting the data into test and train
data to create a machine learning model. 

The models created are Logistic Regression, K-Nearest Neighbours, Support Vector Machine, Decision Tree Classifier and Random Forest Classifier. The use of GridSearch improved the accuracy of all model.

## Analysis

### Comparison
After comparing all the models, it looks like Random Forest Classifier gives the best Accuracy Score.

| Logistic Regression with GridSearch Score | Decision Tree with GridSearch scores | Random Forest with GridSearch scores | K-Nearest Neighbours with GridSearch scores | SVM with GridSearch scores |
|-|-|-|-|-|
| Training Data Score: 0.825 | Training Data Score: 0.890 | Training Data Score: 1.0 | Training Data Score: 0.822 | Training Data Score: 0.824 |
| Testing Data Score: 0.810 | Testing Data Score: 0.882 | Testing Data Score: 0.909 | Testing Data Score: 0.798 |Testing Data Score: 0.805 |

### Random Forest Clasification Report (optimized by GridSearch)
In Exoplanet-Exploration senario, the percision is more important than the recall and looking at the report below, the precision rate(0.84) is greater than recall rate (0.79 ).


![Random Forest Clasification Report](images/RandomForestClasificationReport.png)

## Contributors

- [Helen Amin](https://github.com/helenamin)

## Technology

- ![PythonLogo](images/pythonlogo.png)
