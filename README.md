# sunseeker
Find out how far you have to travel within the US in order to substantially increase the chance of experiencing a sunny day, for a given month in the year. 

For example, it's harder to get a better chance of sunlight in the Boston area than Boston itself. The horizontal red dashed line is the percentage of days with sunlight in the given city. The vertical dashed lines are placed at increments of 60 miles.

![Boston sunlight distance chart](https://i.imgur.com/6oeWoLz.png) 

On the other hand, people who live in detroit do have access to locations within a few hour drive that have a 10 percentage point greater chance of sunlight in January.

![Detroit sunlight distance chart](https://i.imgur.com/LMmPVOj.png) 

Note: this code has several bugs and limitations:
* Not all locations were properly parsed
* Although the percentages calculated here follow the procedure that I understand to be behind the data in pctpos15.dat, the percentages I calculate  are systematically biased down by 1-2 percentage points compared to the official summary table. I haven't had a chance to investigate this, but the bias seems consistent.  
* This analysis only provides information about the predicted percentage of sunny or partly cloudy days in a given month, based on historical meteorological observations. It doesn't account for the amount of solar radiation received by a given location during that period of time. If you're thinking about Vitamin D, an hour of sunlight in LA might do more for you than an hour of sunlight in Seattle.

Sunlight data comes from the NOAA comparative climate dataset:
* https://www.ncdc.noaa.gov/ghcn/comparative-climatic-data ([TSV file here](https://www1.ncdc.noaa.gov/pub/data/ccd-data/pctpos15.dat))

### Other datasets
city-to-city flight data is available in the domestic airline consumer airfare report: 
*  https://www.transportation.gov/policy/aviation-policy/domestic-airline-consumer-airfare-report


# LICENSE
Copyright 2018 J. Nathan Matias

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
