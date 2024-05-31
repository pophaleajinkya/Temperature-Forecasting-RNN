# Temperature-Forecasting-RNN

We will work on a weather forecasting problem, where we have access to a timeseries of data points coming from sensors installed on the roof of a building, such as temperature, air pressure, and humidity, which we use to predict what the temperature will be 24 hours after the last data point collected. This is a fairly challenging problem that exemplifies many common difficulties encountered when working with timeseries.

Until now, the only sequence data we have covered has been text data, for instance the IMDb dataset. But sequence
data is found in many more problems than just language processing. In this notebook, we will be playing with a weather timeseries dataset recorded at the Weather Station at the Max-Planck-Institute for Biogeochemistry in Jena, Germany: http://www.bgc-jena.mpg.de/wetter/.

In this dataset, 14 different quantities (such air temperature, atmospheric pressure, humidity, wind direction, etc.) are recorded every 10 minutes, over several years. The original data goes back to 2003, but we limit ourselves to data from 2009-2016. This dataset is perfect for learning to work with numerical timeseries. We will use it to build a model that takes as input some data from the recent past (a few days worth of data points) and predicts the temperature 24 hours in the future.
