---
layout: page
title: Projects
permalink: /projects
---

## Personal Projects

The source code for these personal projects are on [my GitHub](https://github.com/alanjding).

**TrainingNotebook** \| Jul 2019 - Aug 2019

A Jupyter Notebook that allows me to fetch and extensively analyze my running data from Strava. It can estimate acute and chronic training load as well as provide plots showing different performance metrics. The data fed into these plots can be filtered by traits such as sleep quality and motivation to run which the user provides daily to a questionnaire.

In particular, various streams from my Strava data (time-indexed lists of instantaneous statistics such as heart rate, distance covered, cadence) are pulled. The heart rate stream is ultimately used to arrive at a metric called "Form", measuring training stress with respect to fitness. This is functionality available in existing training analytics software (such as TrainingPeaks); however, I had to recalculate it in this application to do further correlative analyses.

The above objective, formulaic approach to my training data is then combined with user inputted data on sleep quality, sleep time, soreness, and motivation, as well as temperature and dew point data. The application can generate histograms and run Gaussian mixture models on aggregated pace and heart rate stream data. On the other hand, the user inputted data is correlative analyses between any two of these variables, in addition to the run's date, distance, time of day, form, or deviation from expected heart rate. Expected heart rate for a run, knowing its pace, is obtained by converting the pace to a percentile, and getting the heart rate corresponding to that percentile.

The point of the application is to quantify the effectiveness of any training that I do and catch signs of overtraining/burnout earlier (form, drops in performance unrelated to external factors, consistently positive deviation from expected heart rate, etc.)

## Work Projects

**Query and Usage Explorer** \| Jun 2019 - Aug 2019 \| Completed as a technology intern at CAS

Worked with a team of other interns under Agile project management on a data analytics platform with the ability to provide detailed, up-to-date metrics capturing a wide range of aspects about how CAS's customers are using CAS's products. The project was primarily written in Java, Scala, Python, and Groovy. It also leveraged several other industry-standard technologies including Jenkins, Docker, Maven, and Git. Using a Hadoop distributed file system paired with Apache Spark, a big data framework, the platform scales seamlessly, maintaining high performance for complex queries into aspects of the large and ever-growing usage dataset. In the end, the highly anticipated platform would give leadership and data analytics teams at CAS fresh insights on how to better tailor the user experience and performance of their products to their clients' needs.

From a more computer science-oriented viewpoint, at a very high level, the Query and Usage Explorer reads in and parses XML usage data inside of CAS's distributed file system and creates a large graph (the vertices and edges kind) that can be efficiently operated on through distributed graph processing techniques.

## (Selected) Course Projects

**Buffer Overrun Attack** \| Introduction to Programming Systems \| Princeton University

Hacked a sloppily written program by giving it input with executable machine-language instructions inside that gets past the program's input buffer boundary and forces the program to run the user-inputted executable instructions instead of the program's own code.

**Burrows-Wheeler Compression** \| Algorithms and Data Structures \| Princeton University

Implemented the Burrows-Wheeler data compression algorithm, which is a three-step compression algorithm (Burrows-Wheeler transform, move-to-front encoding, Huffman compression) that drastically improves upon the compression ratio of pure Huffman encoding (on the Calgary corpus, Huffman alone achieves a compression rate of 4.7 bits per character, whereas Burrows-Wheeler achieves 2.29 bits/char).
