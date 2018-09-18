#Was just messing around with markdown so made everything into comments 

#*italic*
#**bold**
#***bold italic***

### Just messing around with this video game sales data set from kaggle.com

#* had some trouble originally figuring out the process of uploading data sets

#* Still a work in progress being able to manipulate them

#* The plot isn't meaningful or pretty by any means but just messing around with the process of working with matplotlib and making sure I could get one made for now 

import pandas as pd

import matplotlib.pyplot as plt

data = pd.read_csv('vgsales.csv')

print(data.head())

print(data.describe())

print(data['Publisher'].value_counts())

plt.plot(data['NA_Sales'])

plt.show()
