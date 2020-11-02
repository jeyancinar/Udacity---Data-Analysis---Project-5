# Ford GoBike
by Jeyan Çınar

## Investigation Overview

Ford GoBike is a bike sharing system powered both by Lyft and Ford in San Francisco Bay Area. Thousands of bikes to pick up and drop off anywhere - connecting people to work, friends and their favorite restaurant. Pocket friendly subscriptions and 24/7 available stations make it more compelling to ride. Unfortunately they're not in use anymore - it seems Lyft has pulled away from Ford's project due to some technical problems with the bikes themselves in 2019. But for the sake of this project I'll look into the data from February 2019 to see if I can spot any trends.

## Submission Overview
- exploration_jcinar.ipynb: Main notebook for wrangling & visualization efforts.
- exploration_jcinar.html: Main file for wrangling & visualization efforts.
- slide_deck_jcinar.ipynb: Summary notebook to create a slide show about main findings.
- slide_deck_jcinar.html: Summary file to create a slide show about main findings.
- slide_deck_jcinar,slides.html: Summary slide show about main findings.
- readme.md: This file; summary in plain text.

## Data Set Overview

The data has 174952 entries and 13 rows. These include data in date & time, string and numeric formats.

-   Start & end times indicate when the bike was picked up from & left at the station.
-   Similarly start & end station names are also given.
-   Bike IDs indicate the individual bike identifications.
-   User type indicates if the rider has a subscription or doesn't.
-   Member gender is the gender identifier of the rider.
-   Duration is the length of the trip in minutes.
-   Start & end weekdays indicate the name of the days the trip took place.
-   Similarly start & end hours indicate the time of the days.
-   Member age is calculated by extracting member's birth year given from the data set's year, 2019.

## Outcomes
-   Distributions of age and trip durations don’t have any correlation.
-   Variation around the mean trip duration of 12 minutes is larger in weekends – people prefer shorter trips on work days.
-   Customers tend to have longer trips than subscribers (only by a couple of minutes).
-   Women seem to take longer trips than men, although the mean is still around 12 minutes.
-   People that take trips on weekends seem to have a slightly lower mean ageof 30, where the mean of working days is around 32 – 34.
-  Subscribers and customers have quite similar age distributions, still around the mean of 32.
-   Although the difference is not that significant, females seem to be a couple of years younger than men, having a tighter range of ages.
-   Working hours have a shorter range of trip durations, where 3 and 4 a.m. seem to have wider IQRs.
-   Mean age and variety is around 34 during working hours, but it’s interesting to see a peak of age 42 at 4 a.m.

## Comments

Unfortunately, I wasn't able to find any interesting or surprising interactions between features. Since I had only categorical and completely uncorrelated numeric data, it was hard to find out other aspects of the data set. This study can be expanded with additional information such as station capacities, customer occupations, route analyses or by collecting data from a larger time window.
