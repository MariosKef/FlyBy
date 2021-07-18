# FlyBy
<p align="center">
  <img width="200" height="200" src="images/LogoMakr-0JMFWY.png" />
</p>

<!-- ![](/images/LogoMakr-0DZT22.png) -->

[![Python 3.9.0](https://img.shields.io/badge/python-3.9.0-green.svg?style=plastic)](https://www.python.org/downloads/release/python-390/)


Identify in detail regions of interest that your flight flew over.

This small project helps in identifying (_postflight for now_) areas that you as a passenger flew over, found interesting and would 
like to identify for future reference.
Simply note down the time of an interesting site (lake, city, road, mountain, etc.) and then through this tool find the area you are looking for by searching (for now manually) on the generated map (hovering over the points of the trajectory reveals time) for the time you noted down .

The data is taken from the **tracklogs** of https://flightaware.com/.

## Usage
``map = traj(url, tz)``

``map``

### Example
Enter your flight **tracklog** from flightaware (e.g., search for a flight that has already arrived) in the ``url`` and the time zone in ``tz`` (tz format should be as _Europe/Amsterdam_).

``url = 'https://flightaware.com/live/flight/KLM1573/history/20210715/0635Z/EHAM/LGAV/tracklog'``

``tz = 'Europe/Amsterdam'``

``map = traj(url, tz)``

``map``

![](/images/flyby_1.png)
![](/images/flyby_2.png)

# To-do:
* Automate the process by simply adding the departure date and flight numbers as arguments.
* Give insights on areas around the flight coordinates (within a given radius).
* Turn into cli tool.
