# Space-Time-User-Distribution-Dataset
Olga Ruiz, Juan Sánchez-González, Jordi Pérez-Romero, Oriol Sallent, Irene Vilà

Universitat Politècnica de Catalunya (UPC), Barcelona, Spain

February, 2024


# Overview

This dataset contains the measurements of the number of users connected to each one of the 247 Wifi indoor Access Points (APs) deployed in the Campus Nord of Universitat Politècnica de Catalunya (UPC) in Barcelona. The university campus is a rectangular area of 335 m x 125 m. It comprises 24 buildings that are 3 floors high. The measurements cover a total of 62 days. In addition to the number of users, the dataset also includes the information of the theoretical coverage area of each AP, so that the number of users connected to each AP can be associated to a specific geographical area. 

The following figure shows the area of the Campus where the measurements have been obtained and an example with the evolution of the number of users in one AP during one day.

![image](https://github.com/user-attachments/assets/92444295-39b9-48fc-9225-dffa93ec3659)




# Dataset Contents/Dataset Description

The dataset is composed of the following files:

1) User distribution measurement files:
A total of 62 csv files each one containing the time evolution of the number of connected users per AP for one day in the period from Tuesday 18th April 2023 00:07:30 to Sunday 18th June 2023 23:47:22. Each file is named following the format campus_users_yyyymmdd.csv (e.g. campus_users_20230418.csv) where dd, mm and yyyy represent, respectively, the day, month and year. Each file contains a table with the following three columns: 
- AP_id – The ID of the Wifi AP corresponding to the given data. The IDs are integers ranging from 1 to 247. 
- Time - The timestamp of each measurement specified in the format DayOfTheWeek Month Day hh:mm:ss TimeZone Year (e.g. Tue Apr 18 23:53:03 CEST 2023). 
- Users – The total number of connected users to the AP at the specified time. 

2) Spatial regions files:
Files named as regions_map_floor_0.csv, regions_map_floor_1.csv and regions_map_floor_2.csv, corresponding, respectively, to the ground floor, the first floor and the second floor. Each file contains a matrix of 335 rows and 125 columns. Each element of the matrix is a pixel of 1m x 1m that corresponds to one position in the campus. The value of the pixel is the identifier of the closest AP to the pixel or 0 if the pixel is not associated to any AP.

# Getting Started

All the files in the dataset are provided in csv format, so there is no specific software or prerequisites to read them. The following figure shows a snapshot of one of the files included in the dataset.

![image](https://github.com/user-attachments/assets/dd779f26-3d4e-44ff-a47f-5c76a2fb51f7)

# Download & Usage

Dataset can be found in https://github.com/VERGE-PROJECT/Space-Time-User-Distribution-Dataset 

# Citation

Please cite the following paper in any publications in which you used the dataset:
O. Ruiz, J. Sánchez-González, J. Pérez-Romero, O. Sallent, I. Vilà, "Space and time user distribution measurements dataset in a university campus", Computer Networks, Vol. 243, 2024, 110329. https://doi.org/10.1016/j.comnet.2024.110329  



