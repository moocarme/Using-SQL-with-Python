#Using the Google Geocoding API with a Database and Visualizing data on Google Map

In this project, I use the Google geocoding API
to clean up some user-entered geographic locations and then place
the data on a Google Map.

In the first phase I take our input data in the file
(where.data) and read it one line at a time, and retreive the
geocoded response and store it in a database (geodata.sqlite).
Before using the geocoding API, we simply check to see if
we already have the data for that particular line of input.

Once some data is loaded into geodata.sqlite, the data is 
visualized using the (geodump.py) program. This
program reads the database and writes tile file (where.js)
with the location, latitude, and longitude in the form of
executable JavaScript code. 

The file (where.html) consists of HTML and JavaScript to visualize 
a Google Map.  It reads the most recent data in where.js to get 
the data to be visualized.  
