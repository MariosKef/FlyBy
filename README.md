# FlyBy
[![Python 3.9.0](https://img.shields.io/badge/python-3.9.0-green.svg?style=plastic)](https://www.python.org/downloads/release/python-390/)


Identify in detail regions of interest that your flight flew over.

This small project helps in identifying (_postflight for now_) areas that you as a passenger flew over, found interesting and would 
like to identify for future reference.

The data is taken from the **tracklogs** of https://flightaware.com/.

## Usage
``map = traj(url, tz)``

``map``

### Example
Enter your flight **tracklog** from flightaware (e.g., search for KL1573 that has already arrived) in the ``url`` and the time zone in ``tz`` (tz format should be as _Europe/Amsterdam_).

``url = 'https://flightaware.com/live/flight/KLM1573/history/20210715/0635Z/EHAM/LGAV/tracklog'``

``tz = 'Europe/Amsterdam'``

``map = traj(url, tz)``

``map``

![](/images/flyby_1.png)
![](/images/flyby_2.png)
