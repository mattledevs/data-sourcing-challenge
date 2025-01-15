# Background
Here we prepare a dataset for a prediction system that will help the NOOA Space Weather Prediction CenterLinks to an external site. predict Geomagnetic Storms (GSTs).

These storms are caused by so-called Coronal Mass Ejections (CMEs), which are a massive bursts of plasma emitted from the Sun in irregular intervals, that Earth's magnetic shield fortunately renders harmless to us. However, this interaction with the magnetic shield can still create so-called Geomagnetic Storms (which also cause the Northern and Southern Lights) that can be harmful to electronic devices such as satellites, GPS systems, and essential parts of our powergrids.

NASA and the Space Weather Prediction Center operate a number of measuring satellites that collect data on CMEs. This data is then used to warn powergrid operators and GPS system operators ahead of time, so that they can make necessary adjustments.

# Location of Repo
[https://github.com/mattledevs/data-sourcing-challenge](https://github.com/mattledevs/data-sourcing-challenge)

# NASA API KEY
To run code, you must provide your own NASA API Key in the form of the variable "NASA_API_KEY" in your .env file. You can sign up for a NASA API Key here:
[https://api.nasa.gov/](https://api.nasa.gov/)

# Methodology

Part 1, we request and prep the CME data and in Part 2, we request GST data, both from NASA API. Prepping these data sets, allows us to in Part 3, merge and clean the data based off of gstID and CME_ActivityID for GST. 

We then use a the describe function to predict the mean and median time that it takes for a CME to cause a GST.
