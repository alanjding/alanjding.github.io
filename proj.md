---
layout: page
title: Projects
permalink: /projects
---

## Personal Projects

The source code for my personal projects are on [my GitHub](https://github.com/alanjding).

**TrainingTracker** \| Jul 2019 - Aug 2019
A Jupyter Notebook that allows me to fetch and extensively analyze my running data from Strava. It can estimate acute and chronic training load as well as provide plots showing different performance metrics. The data fed into these plots can be filtered by traits such as sleep quality and motivation to run which the user provides daily to a questionnaire.

In particular, various streams from my Strava data (time-indexed lists of instantaneous statistics such as heart rate, distance covered, cadence) are pulled. The heart rate stream is ultimately used to arrive at a metric called "Form", measuring training stress with respect to fitness. This is functionality available in existing training analytics software (such as TrainingPeaks); however, I had to recalculate it in this application to do further correlative analyses.

The above objective, formulaic approach to my training data is then combined with user inputted data on sleep quality, sleep time, soreness, and motivation, as well as temperature and dew point data. The application can generate histograms and run Gaussian mixture models on aggregated pace and heart rate stream data, which could include the whole data set, or runs on a day whose sleep time, sleep quality, soreness, motivation, TD (temperature + dew point), or the date itself fall within a specified range. The other aspect of the user inputted data is correlative analyses between any two of these variables, in addition to the run's date, distance, time of day, form, or deviation from expected heart rate. Expected heart rate for a run, knowing its pace, is obtained by converting the pace to a percentile, and getting the heart rate corresponding to that percentile.

The point of the application is to quantify the effectiveness of any training that I do and catch signs of overtraining/burnout earlier (form, drops in performance unrelated to external factors, consistently positive deviation from expected heart rate, etc.)

## Work Projects

**Query and Usage Explorer** \| Jun 2019 - Aug 2019 \| Completed as a technology intern at CAS

## Course Projects
