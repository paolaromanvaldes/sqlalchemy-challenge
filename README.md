# sqlalchemy-challenge

## Instructions

Congratulations on planning your holiday vacation in Honolulu, Hawaii! To assist with your trip planning, you've decided to perform a climate analysis of the area using Python and SQLAlchemy. Additionally, you will design a Flask API based on the queries developed during the analysis. Below are the detailed instructions to guide you through both parts of the project.

### Part 1: Analyze and Explore the Climate Data

1. **Connect to Database:**
   - Use the SQLAlchemy `create_engine()` function to connect to your SQLite database.

2. **Reflect Tables:**
   - Use the SQLAlchemy `automap_base()` function to reflect your tables into classes.
   - Save references to the classes named `station` and `measurement`.

3. **Create Session:**
   - Link Python to the database by creating a SQLAlchemy session.
   - **IMPORTANT:** Remember to close your session at the end of your notebook.

4. **Precipitation Analysis:**
   - Find the most recent date in the dataset.
   - Retrieve the previous 12 months of precipitation data from that date.
     - Select only "date" and "prcp" values.
     - Load the query results into a Pandas DataFrame.
     - Set column names explicitly.
     - Sort the DataFrame values by "date."
   - Plot the results using the DataFrame plot method.
   - Use Pandas to print the summary statistics for the precipitation data.

5. **Station Analysis:**
   - Design a query to calculate the total number of stations in the dataset.
   - Find the most-active stations.
     - List the stations and observation counts in descending order.
     - Identify the station with the greatest number of observations.
   - Calculate the lowest, highest, and average temperatures for the most-active station.
   - Query the previous 12 months of temperature observation (TOBS) data for the most-active station.
   - Plot the results as a histogram with bins=12.

6. **Close Session:**
   - Close your session.

### Part 2: Design Your Climate App


Follow these instructions to complete your climate analysis and design your Flask API for a seamless trip planning experience. Safe travels!