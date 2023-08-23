The Module 10 Challenge uses Python and SQLAlchemy to do a basic climate analysis and data exploration with SQLAlchemy ORM queries, Pandas, and Matplotlib. The Challenge is divided into two parts:
* Part 1: Analyze and Explore Climate Data
* Part 2: Design Climate App

**Part 1: Analyze and Explore the Climate Data**
**Precipitation Analysis**
* Find the most recent date in the dataset.
* Using that date, get the previous 12 months of precipitation data by querying the previous 12 months of data.
* Select only the "date" and "prcp" values.
* Load the query results into a Pandas DataFrame. Explicitly set the column names.
* Sort the DataFrame values by "date".
* Plot the results by using the DataFrame plot method
* Use Pandas to print the summary statistics for the precipitation data

**Station Analysis**
* Design a query to calculate the total number of stations in the dataset.
* Design a query to find the most-active stations (that is, the stations that have the most rows).
* List the stations and observation counts in descending order.
* Design a query that calculates the lowest, highest, and average temperatures that filters on the most-active station id found in the previous query.
* Design a query to get the previous 12 months of temperature observation (TOBS) data.

**Part 2: Design Climate App**
Displays a precipitation route that:
* Returns json with the date as the key and the value as the precipitation
* Only returns the jsonified precipitation data for the last year in the database

Displays a stations route that:
* Returns jsonified data of all of the stations in the database

Displays a tobs route that:
* Returns jsonified data for the most active station (USC00519281)
* Only returns the jsonified data for the last year of data
