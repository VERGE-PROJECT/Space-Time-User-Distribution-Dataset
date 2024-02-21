# Space-Time-User-Distribution-Dataset
Authors: Olga Ruiz, Juan Sánchez-González, Jordi Pérez-Romero, Oriol Sallent, Irene Vilà\n
Universitat Politècnica de Catalunya (UPC), Barcelona, Spain
February, 2024


The dataset contains the measurements of the number of users connected to each one of the 247 Wifi indoor Access Points (APs) deployed in the Campus Nord of Universitat Politècnica de Catalunya (UPC) in Barcelona. The university campus is a rectangular area of 335 m x 125 m. It comprises 24 buildings that are 3 floors high. The measurements cover a total of 62 days. In addition to the number of users, the dataset also includes the information of the theoretical coverage area of each AP, so that the number of users connected to each AP can be associated to a specific geographical area. 
The dataset is composed of the following files:

1) User distribution measurement files:
A total of 62 csv files each one containing the time evolution of the number of connected users per AP for one day in the period from Tuesday 18th April 2023 00:07:30 to Sunday 18th June 2023 23:47:22. Each file is named following the format campus_users_yyyymmdd.csv (e.g. campus_users_20230418.csv) where dd, mm and yyyy represent, respectively, the day, month and year. Each file contains a table with the following three columns: 
- AP_id – The ID of the Wifi AP corresponding to the given data. The IDs are integers ranging from 1 to 247. 
- Time - The timestamp of each measurement specified in the format DayOfTheWeek Month Day hh:mm:ss TimeZone Year (e.g. Tue Apr 18 23:53:03 CEST 2023). 
- Users – The total number of connected users to the AP at the specified time. 

2) Spatial regions files:
Files named as regions_map_floor_0.csv, regions_map_floor_1.csv and regions_map_floor_2.csv, corresponding, respectively, to the ground floor, the first floor and the second floor. Each file contains a matrix of 335 rows and 125 columns. Each element of the matrix is a pixel of 1m x 1m that corresponds to one position in the campus. The value of the pixel is the identifier of the closest AP to the pixel or 0 if the pixel is not associated to any AP.

