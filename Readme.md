# Max Temperature Investigation

**Purpose**

[Dark Sky](https://darksky.net/) (previously forecast.io) specializes in weather forecasting and visualization.  This is an exploratory analysis on the maximum temperature per day for five different cities.

**Learning Objectives**

* Interface with an API to collect data
* Calculate descriptive statistics
* Generate autocorrelation plots

**Method**

Maximum temperature per day was obtained using the Dark Sky [API](https://api.darksky.net/).  Temperature data was originally captured June 23rd, 2016 to July 22nd, 2016 and was stored in a SQLite3 database.

**Results**

* **Max Temperature Details for Seattle:**
  * Max Max Temperature: 76.76
  * Max Temperature Range: 12.63
  * Mean Max Temperature: 70.03
  * Max Temperature Variance: 12.93

* **Max Temperature Details for Washington:**
  * Max Max Temperature: 103.42
  * Max Temperature Range: 30.76
  * Mean Max Temperature: 89.65
  * Max Temperature Variance: 60.91

* **Max Temperature Details for Minneapolis:**
  * Max Max Temperature: 104.03
  * Max Temperature Range: 34.44
  * Mean Max Temperature: 84.46
  * Max Temperature Variance: 82.44

* **Max Temperature Details for Denver:**
  * Max Max Temperature: 91.37
  * Max Temperature Range: 16.21
  * Mean Max Temperature: 84.57
  * Max Temperature Variance: 16.31

* **Max Temperature Details for Cleveland:**
  * Max Max Temperature: 98.50
  * Max Temperature Range: 26.46
  * Mean Max Temperature: 83.24
  * Max Temperature Variance: 59.33

![alt text](https://raw.githubusercontent.com/silkaitis/MaxTemp/master/Max%20Temperature%20vs%20Day.png)

![alt text](https://raw.githubusercontent.com/silkaitis/MaxTemp/master/Autocorrelation%20-%20Seattle.png)

![alt text](https://raw.githubusercontent.com/silkaitis/MaxTemp/master/Autocorrelation%20-%20Minneapolis.png)

![alt text](https://raw.githubusercontent.com/silkaitis/MaxTemp/master/Autocorrelation%20-%20Denver.png)

![alt text](https://raw.githubusercontent.com/silkaitis/MaxTemp/master/Autocorrelation%20-%20Cleveland.png)

![alt text](https://raw.githubusercontent.com/silkaitis/MaxTemp/master/Autocorrelation%20-%20Washington.png)

**Interpretation**

Minneapolis had the largest change in maximum temperature over the 30 day period.  Washington has the largest maximum temperature delta in a single day with a 22.16 degree change.  Autocorrelation plots illustrate a lag 1 correlation which is reasonable since weather one day is dependent upon the previous day.  

**Code**

* MaxTemp.ipynb ~ API query, data storage and analysis
