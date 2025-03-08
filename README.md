# Ex.No: 01A PLOT A TIME SERIES DATA

###  Date: 03/08/2025

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity temperature.

# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.

# PROGRAM:

```
import pandas as pd
import matplotlib.pyplot as plt
file_path='/content/Gold Price (2013-2023).csv'
data=pd.read_csv(file_path)
data['Date'] = pd.to_datetime(data['Date'])
data.set_index('Date', inplace=True)
plt.figure(figsize=(10, 6))
plt.plot(data.index, data['Price'], label='Gold Price Today', color='blue')
plt.title('Gold Price Today Over Time')
plt.xlabel('Date')
plt.ylabel('Gold Price')
plt.grid(True)
plt.legend()
plt.show()
```

# OUTPUT:

![Time series output](https://github.com/user-attachments/assets/3120ca02-dbce-403a-a3dc-f572cd4d77a8)

![Time series output 1](https://github.com/user-attachments/assets/2dd2783f-ec69-4b38-820a-99371501b311)


# RESULT:

Thus we have created the python code for plotting the time series of given data.
