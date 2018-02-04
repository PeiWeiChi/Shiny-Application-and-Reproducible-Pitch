Shiny Application and Reproducible Pitch
========================================================
author: Pei Wei Chi 
date: 2/4/2018
autosize: true

Shiny Application - Air Passengers
========================================================

This a Shiny-App for Coursera Assignment, please refer to the hyperlink below for the application https://williams33307.shinyapps.io/ShinyApplicationandReproduciblePitch/

The shiny package in R is using to make this app and upload to the Shinyapps cloud



Data set
========================================================
The resourse of data is AirPassengers from R dataset

##Monthly Airline Passenger Numbers 1949-1960

Description: The classic Box & Jenkins airline data. Monthly totals of international airline passengers, 1949 to 1960.

Source: Box, G. E. P., Jenkins, G. M. and Reinsel, G. C. (1976) Time Series Analysis, Forecasting and Control. Third Edition. Holden-Day. Series G.


Data structure
========================================================


```r
AirPassengers
```

```
     Jan Feb Mar Apr May Jun Jul Aug Sep Oct Nov Dec
1949 112 118 132 129 121 135 148 148 136 119 104 118
1950 115 126 141 135 125 149 170 170 158 133 114 140
1951 145 150 178 163 172 178 199 199 184 162 146 166
1952 171 180 193 181 183 218 230 242 209 191 172 194
1953 196 196 236 235 229 243 264 272 237 211 180 201
1954 204 188 235 227 234 264 302 293 259 229 203 229
1955 242 233 267 269 270 315 364 347 312 274 237 278
1956 284 277 317 313 318 374 413 405 355 306 271 306
1957 315 301 356 348 355 422 465 467 404 347 305 336
1958 340 318 362 348 363 435 491 505 404 359 310 337
1959 360 342 406 396 420 472 548 559 463 407 362 405
1960 417 391 419 461 472 535 622 606 508 461 390 432
```


Data usage
=======================================================
It's a time-serious table in R, the left most side is the year and the top is month.
In order to extract data, we have to use "window" function, otherwise, the specifict data can't be obtain.
window is a generic function which extracts the subset of the object x observed between the times start and end. If a frequency is specified, the series is then re-sampled at the new frequency.


App discreption
=======================================================


In the user interface, you can slide the bar to select a specific year that you want to know, the range is from 1949 to 1960. After you select, the figur in the right side will show the distribution of passengers from Jan. to Dec. in the year you selected.


