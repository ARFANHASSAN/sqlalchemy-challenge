
# SQLAlchemy Challenge:

1. Establish a fresh repository for the project, naming it "sqlalchemy-challenge." Ensure that this assignment is not incorporated into any pre-existing repositories.

2. Duplicate the recently created repository onto your local computer by executing the clone command.

3. Include your Jupyter notebook and app.py files in this directory. These scripts will serve as the primary ones to execute for the analysis.


# Exploration and Analysis of Climate:

* Utilize the supplied initial notebook and hawaii.sqlite files to fulfill your climate analysis and explore the data.
* Select a commencement date and conclusion date for your journey.
* Utilize SQLAlchemy's create_engine to establish a connection with your SQLite database.
* Employ SQLAlchemy's automap_base() to reflect the tables into classes, and retain references to these classes as Station and Measurement.


# Analysis of Precipitation:
 
* Devise a query to fetch precipitation data from the past 12 months.
* Choose solely the date and precipitation (prcp) values.
* Load the results of the query into a Pandas DataFrame and designate the     date column as the index.
* Arrange the values in the DataFrame in ascending order based on the date.
* Visualize the outcomes using the plot method of the DataFrame.

# Station Analysis

Create a query to determine the total count of stations.

Formulate a query to identify the stations with the highest activity level.

List the stations along with their observation counts, arranged in descending order.

Identify the station that records the maximum number of observations.

Tip: You might need to employ functions like func.min, func.max, func.avg, and func.count in your queries.

Develop a query to fetch the temperature observation data (tobs) for the last 12 months.

Filter the results based on the station with the highest number of observations.

Visualize the findings by generating a histogram with 12 bins.


##  Climate App 

Use FLASK to create your routes.

# Routes

/

Home page.

List all routes that are available.

/api/v1.0/precipitation


Transform the query results into a dictionary with date as the key and prcp as the corresponding value.

Provide the JSON representation of your dictionary.

/api/v1.0/stations

Return a JSON list of stations from the dataset.
/api/v1.0/tobs


Retrieve the dates and temperature observations for a year preceding the last data point.

Present a JSON list of Temperature Observations (tobs) for the prior year.
/api/v1.0/<start> and /api/v1.0/<start>/<end>

Provide a JSON list containing the minimum temperature (TMIN), average temperature (TAVG), and maximum temperature (TMAX) for a specified start date or a start-end range.

For a given start date, compute TMIN, TAVG, and TMAX for all dates greater than or equal to the start date.

For a given start and end date, calculate TMIN, TAVG, and TMAX for dates falling within the inclusive range of the start and end dates.

