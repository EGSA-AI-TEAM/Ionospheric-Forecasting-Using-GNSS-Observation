# :hourglass_flowing_sand: VTech Time Series Prediction
 Building and developing a time series deep learning model to predict the VTech (Vertical Total Electron Content) which are the total number of free electrons relesed by the ionisation of the ionosphere caused by solar activities such as solar storms, solar winds and solar flares. For this model we obtained data from 2 sources:
- [OMNIWeb Data Explorer](https://omniweb.gsfc.nasa.gov/form/dx1.html)
- Dataset provided from the EgSA for the years 2022,2023 and half of 2024



![image](https://github.com/user-attachments/assets/67c14c54-00ba-47d7-8712-32fb64394c06)


# :open_file_folder: Dataset
## We collected data from the 2 resources listed above. Each contained different parameters depending on the available readings. 
- The dataset obtained from the OMNIWeb we specified the time span from Jan 2022 to May 2024 sampled every hour, the paramaters we needed were:
![image](https://github.com/user-attachments/assets/0cdeb21d-78b4-4cfb-ac2b-7e5994a0c511)

- The dataset obtaned from the EgSA had many parameters as it was obtained from the readings of the agencie's ground station, it is sampled at 2 reading per second:
![EgSA Data](https://github.com/user-attachments/assets/c70ac9e8-7185-4f2b-b2ea-7a554d2145a1)

  
## 🔄 Data Cleaning:
### 1. The data obtained from the OMNIWeb, we found that there are many outliers in the data, and in order to remove the outliers we did the following:
- We took the average reading from the rows above and below the outling rows and replaced the outling numbers.
### 2. Due to the vast differences in sample rate between the 2 data resources we had to resample the datasets in order to be able to concatenate them in one combined dataset we decided to do the following:
-  In the data given to us by the EgSA we took the average reading for each hour in order to be able to concatenate this data with the OMNIWeb data and create a dataset we can fit into our model. 

# 🤝🏼 Contributers:
|  Name |
| --- |
| Abdulrahman Hisham |
| Hamza Elghonemy |
| Jannat Allah Sabry |
| Youssef Husseiny |








