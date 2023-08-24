The Module 10 Challenge uses Python and SQLAlchemy to do a basic climate analysis and data exploration with SQLAlchemy ORM queries, Pandas, and Matplotlib. The Challenge is divided into two parts:
* **Part 1:** Analyze and Explore Climate Data
* **Part 2:** Design Climate App

**Part 1: Analyze and Explore the Climate Data**
**Precipitation Analysis**
* Creates a query that finds the most recent date in the dataset (8/23/2017)
* Creates a query that collects only the date and precipitation for the last year of data without passing the date as a variable
* Saves the query results to a Pandas DataFrame to create date and precipitation columns
* Sorts the DataFrame by date
* Plots the results by using the DataFrame plot method with date as the x and precipitation as the y variables
* Uses Pandas to print the summary statistics for the precipitation data

**Station Analysis**
* Creates a query to calculate the total number of stations in the dataset
* Creates a query that correctly lists the stations and observation counts in descending order and finds the most active station (USC00519281)
* Creates a query that correctly finds the min, max, and average temperatures for the most active station (USC00519281).
* Creates a query to get the previous 12 months of temperature observation (TOBS) data that filters by the station that has the greatest number of observations
* Saves the query results to a Pandas DataFrame

**Part 2: Design Climate App**

Correctly plot a histogram with bins=12 for the last year of data using tobs as the column to count
Displays a precipitation route that:
* Returns json with the date as the key and the value as the precipitation
* Only returns the jsonified precipitation data for the last year in the database

Displays a stations route that:
* Returns jsonified data of all of the stations in the database

Displays a tobs route that:
* Returns jsonified data for the most active station (USC00519281)
* Only returns the jsonified data for the last year of data

Displays a start route that:
* Accepts the start date as a parameter from the URL
* Returns the min, max, and average temperatures calculated from the given start date to the end of the dataset

Displays a start/end route that:
* Accepts the start and end dates as parameters from the URL
* Returns the min, max, and average temperatures calculated from the given start date to the given end date
