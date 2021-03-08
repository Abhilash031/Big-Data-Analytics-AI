# Big-Data-Analytics
BDA Technical Project


Abhilash Kumar (M.Sc. Big Data Analytics and AI)

Abstract:
=========
This work has been carried out to analyse the covid-19 data on the number of infected as well deaths worldwide and to make 
it understandable using Arti?cial Intelligence and Big Data Analysis.We will also try to build AI model using Machine 
Learning techniques which should be able to predict the number infected people based on the trend available. For this purpose
we are using time series datasets available at Johns Hopkins GitHub repository - https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data

Introduction:
============
The project is aimed to perform data processing and its analysis using Big Data tools so that the Covid data can be visualised. At the same
time few important aspects of analysis like county wise depiction of data, doubling rate determination and predictions are performed on the
data.

Three datasets related to number of confirmed cases, deaths and recovered cases are studied and explored and then merged for specific
country using Spark on Databricks and visualised using different plots.

Doubling rate determination is performed on number of impacted cases for a specific country and plotted for easy understanding.

Description Section:
====================
The code has been performed on IPython notebook under Databricks. Notebook is available with name L00151343_Technical_Project_V0.5
under GitHub. Mostly all the dataset operations has been performed on Spark however at some places we have used Pandas dataframe
capabilities to achieve the intended goal.

I.   First all the three datasets are extracted on Spark Dataframe.
II.  Original dataset came as dates as columns where every date is a column and a number within that column represent the infected/
deaths/recovered cases.
III. Datasets are processed so that the we created a single date column under which we have all the dates as different rows.
IV.  Values are summed for every country so that we have a number for a specific country and date in the dataframe.
V.   Sql queries are run on dataframe to show datewise counts. Also rows are selected for specific country.
VI.  Graphs are plotted for few countries to show the trends of infected/deaths/recovered people.
VII. Datframes are joined to show the 3 cases for specific country together.
VIII. Doubling rate determination of infected people are plotted.
IX.  Regression model is constructed for the trends to predict numbers in future.
X.   Correlation coefficients are calculated for the 3 numbers (Infected, deaths and Recovered).