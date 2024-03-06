# Weather-Mini-Analysis
#This is a Weather Sensor value Analysis based of Min.Temp, Max.Temp, Rateof Evaporation, Humidity and Rainfall
#I displayed the dataset
#I analysed the dataset for Unique values
#I analysed the dataset for various data per column
#I used the matplot. Library to plot the function of (x)Index number representing days against (y) Min Temp

# Weather Dataset CSV
import pandas as pd
from matplotlib import pyplot as plt
data = pd.read_csv(r"\Users\SAMMY\Downloads\weather.csv")
print(data)

plt.plot(data.index, data.MinTemp)
plt.title("Weather Stats")
print(data)
plt.show()

##DISPLAY DATA
#print(data.index)
#print(data.head)
#print(data.shape)
#print(data.columns)
#print(data.count)

#Data Analysis
#1. Find unique values in "rainfall" in the data
##Extracting Unique Values

#print(data.Rainfall.unique())

##Display number of unique values for the entire data set

#print(data.nunique())

##Data Count Functions for entire Dataset
#print(data.count())

##Display and Count Data count for Single column
#print(data.Evaporation.value_counts())

##Data Information
#print(data.info)

#Data Set Filtering
#print(data.head (2))
#print(data.Rainfall[filter.Rainfall==4.4])






