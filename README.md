# Heart Disease Prediction Modelling

## Introduction
Given our preliminary data exploration conducted with the Cleveland Heart Disease data set (more on this below), we initially chose to use 4 variables to use when building a classifier that would be designed to predict whether or not a patient has heart disease. However, due to our limited knowledge at this time, we are not able to use the "thal" variable (indicating the status of the patient's thalassemia (a blood disorder)) since it is a categorical variable and can't be used in a KNN classifier. As such we will be using the following 3 numerical variables to build our KNN classifier:

1. Maximum heart rate achieved by the patient (bpm)
1. Age of the patient
1. Exercise-induced ST depression (measured by ECG)
---
As found in a 16-year study of initially healthy men, "maximal exercise-induced heart rate [is] associated with cardiovascular mortality" (Sandvik et al.). Age has also been found to impact a patient's risk of developing heart disease, as "[h]eart disease is much more common in older age" (Nutrition Health Review 14). Lastly, ST depression can "indicate health conditions" related to the patient's heart health (Rowden & Goodwin). Therefore, we chose these variables as they were found to have an association with our response variable (diagnosis) both in previous research as well as our preliminary data analysis.

The question we are trying to answer with this predictive data analysis below is, given the stated variables, can we predict if a patient has heart disease?

---
To answer this question, we will be using the Cleveland Heart Disease data set provided by Detrano et al., which contains biological information of potential heart disease patients at the Cleveland Clinic Foundation. In the entire data set, 139 of the patients were diagnosed with heart disease while 164 were not.

---
## Methods
First, we load the tidyverse package to be able to perform data analysis and visualization, along with the tidymodels package which is used for classification. We also load the gridExtra package which is used for our visualisations. This data analysis requires that the tidyverse, tidymodels, ggmosaic and gridExtra R packages be downloaded.

Later on in the methods we use ggmosaic, an extension library to ggplot, to create a visualisation of our data analysis. Thus we first had to install ggmosaic locally in order to work with it. To do that, we ran the following code in the console (right click on cell -> new console for notebook):

---
Run install.packages("remotes", lib = "packages") to install the remotes package, which is used to download packages from GitHub, into a local folder called "packages" (need to create that folder first otherwise it won't write)
Run remotes::install_github("haleyjeppson/ggmosaic", lib = "packages") to install ggmosaic from its location on GitHub using remotes into the local packages folder
Use library(ggmosaic, lib.loc = "packages") to load ggmosaic from the local folder into the R notebook
Note: ggmosaic requires that htmltools be version 0.5.7 or later. If an older version is installed, run install.packages("htmltools") in the console to update it (NOT locally) to the latest version.

The kernel will need to be restarted after installing all of these packages in order for the code below to load ggmosaic.


Project for DSCI 100
