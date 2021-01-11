# delay-expectations
*Allison Merritt, Nov 2020*

What are the chances of my flight being delayed? / digging around in US domestic flights public data 2018-2020


### Part 1: Data collection
Notebook:  [![nbviewer](https://img.shields.io/badge/render%20on-nbviewer-orange.svg)](https://nbviewer.jupyter.org/github/atmerritt/delay-expectations/blob/scribbles/flights_data_scrape.ipynb?flush_cache=true)


### Part 2: Data exploration
Goal: play around with the data -- figure out when flights are delayed, and what drives any trends or patterns that emerge.

![alt text](https://github.com/atmerritt/delay-expectations/blob/scribbles/2018_flights_timeofday.png?raw=true)

Notebook: [![nbviewer](https://img.shields.io/badge/render%20on-nbviewer-orange.svg)](https://nbviewer.jupyter.org/github/atmerritt/delay-expectations/blob/scribbles/flight_delays_data_explore.ipynb?flush_cache=true)


### Part 3: Classifying flights
Goal: using an ExtraTrees model, try to predict whether a flight will be delayed using basic information available at the time of booking (flight time, day, month, airline, origin and destination). 

![alt text](https://github.com/atmerritt/delay-expectations/blob/scribbles/2018_summary.png?raw=true)

Notebook: [![nbviewer](https://img.shields.io/badge/render%20on-nbviewer-orange.svg)](https://nbviewer.jupyter.org/github/atmerritt/delay-expectations/blob/scribbles/flights_classifier_extratrees.ipynb?flush_cache=true)
