## Lab 3 - Python

### Python Environment Preparation
```
C:\Users\n_j\Downloads\iot-master\lesson3> pip install jdcal astral geopy pytz psutil
```
### julian
```
C:\Users\n_j\Downloads\iot-master\lesson3> py julian.py
Calendar Date: 2023-04-03
Julian Date: 2460037.5
Modified Julian Date: 60037.0
```
### date_example
```
C:\Users\n_j\Downloads\iot-master\lesson3> py date_example.py
Date: 2023-04-03
Date: 04-03-23
Day of Week: Monday
Month: April
Year: 2023
75 days after the first day of classes
31 days before the last day of classes
```
### datetime_example
```
C:\Users\n_j\Downloads\iot-master\lesson3> py datetime_example.py
2023-04-03 10:35:40.058815
2023-04-03 10:35:40.058815
2023-04-03 14:35:40.058815
1680532540.0598469
Mon Apr  3 10:35:40 2023
2023-04-03 10:35:40.059847
2023-04-03 14:35:40.059847
```
### time_example
```
C:\Users\n_j\Downloads\iot-master\lesson3> py time_example.py
Mon Apr  3 10:35:55 2023
```
### sun
```
C:\Users\n_j\Downloads\iot-master\lesson3> py sun.py "New York"
Information for New York/USA

Timezone: US/Eastern
Latitude: 40.72; Longitude: -74.00

Dawn:    2023-04-03 06:08:38.900946-04:00
Sunrise: 2023-04-03 06:36:50.523610-04:00
Noon:    2023-04-03 12:59:28-04:00
Sunset:  2023-04-03 19:22:24.163265-04:00
Dusk:    2023-04-03 19:50:40.477918-04:00
```
### coordinates
```
C:\Users\n_j\Downloads\iot-master\lesson3> py coordinates.py "Samuel C. Williams Library"
Samuel C. Williams Library, Field House Road, Hoboken, Hudson County, New Jersey, 07030, United States
(40.74480675, -74.02532861159351)
```
### address
```
C:\Users\n_j\Downloads\iot-master\lesson3> py address.py "40.74480675, -74.02532862031404"
Samuel C. Williams Library, Field House Road, Hoboken, Hudson County, New Jersey, 07030, United States
(40.74480675, -74.02532861159351)
```
### cpu
```
C:\Users\n_j\Downloads\iot-master\lesson3> py cpu.py
The number of physical cores =  8
The number of logical CPUs =  16
The utilization per second as a percentage for each CPU
[0.0, 0.0, 1.6, 1.6, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 6.2, 3.1, 0.0, 0.0, 0.0, 0.0]
```
### battery
```
C:\Users\n_j\Downloads\iot-master\lesson3> py battery.py
sbattery(percent=43, secsleft=14012, power_plugged=False)
```
### documentstats
```
C:\Users\n_j\Downloads\iot-master\lesson3> py documentstats.py document.txt
Word Count: 1343
Top Ten Words: [('our', 26), ('their', 20), ('has', 20), ('he', 19), ('them', 15), ('these', 13),
('have', 11), ('we', 11), ('us', 11), ('people', 10)]
```
