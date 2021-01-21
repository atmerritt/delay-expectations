# delay-expectations
*Allison Merritt, Jan 2021*


For years, whenever I have booked a flight to go see my family, attend a conference or workshop, or go on vacation, there has been one travel tip embedded at the center of my planning: earlier flights are more likely to depart on-time.

Honestly, though, this is a belief built up by noticing that when I flew earlier in the day things just seemed to go a bit more smoothly. And sometimes I wonder whether it's even remotely correct -- after all, the bad experiences (delayed or cancelled flights) are more memorable than the good, so I'm not sure how far I should really trust my own memory to guide me. Plus, taking earlier flights means waking up earlier in the morning, which is ... not my favorite thing.

So, finally, I've decided to answer this question once and for all. Are early flights really more reliable? Or have I been subjecting myself to early morning alarm clocks for nothing?

### Part 1: Data collection
**Goal:** Build a Selenium WebDriver to scrape public domestic flights data available from the [Bureau of Transportation Statistics](https://www.transtats.bts.gov/Tables.asp?DB_ID=120&DB_Name=Airline%20On-Time%20Performance%20Data&DB_Short_Name=On-Time).

Notebook:  [![nbviewer](https://img.shields.io/badge/render%20on-nbviewer-orange.svg)](https://nbviewer.jupyter.org/github/atmerritt/delay-expectations/blob/scribbles/flights_data_scrape.ipynb?flush_cache=true)


### Part 2: Data exploration
**Goal:** Play around with the flights data -- use data visualization and descriptive statistics to figure out when flights are delayed, and what drives any trends or patterns that emerge. The notebook can be viewed here: [![nbviewer](https://img.shields.io/badge/render%20on-nbviewer-orange.svg)](https://nbviewer.jupyter.org/github/atmerritt/delay-expectations/blob/scribbles/flight_delays_data_explore.ipynb?flush_cache=true)

![alt text](https://github.com/atmerritt/delay-expectations/blob/scribbles/2018_flights_timeofday.png?raw=true)


### Part 3: Classifying flights
**Goal:** Using an ExtraTrees model, try to classify flights as delayed vs on-time using basic information available at the time of booking (flight time, day, month, airline, origin and destination) and reproduce trends revealed during the data exploration stage. Dig into ExtraTrees models, scoring metrics, and hyperparameter optimization using GridSearch. Apply model trained on 2018 data to both 2019 and 2020, and compare with a "dummy" model for reference.

The notebook can be viewed here: [![nbviewer](https://img.shields.io/badge/render%20on-nbviewer-orange.svg)](https://nbviewer.jupyter.org/github/atmerritt/delay-expectations/blob/scribbles/flights_classifier_extratrees.ipynb?flush_cache=true) 

![alt text](https://github.com/atmerritt/delay-expectations/blob/scribbles/2018_summary.png?raw=true)
