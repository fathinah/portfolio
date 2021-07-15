---
title: Anomaly Detection
layout: page
---

## Inspiration

Started from the problem where data ingestion seemed running ok but it actually failed is indicated by the amount of data present in the datalake. We tried to solve the bottleneck to improve the teams efficiency. As a data enginner intern in OVO, I worked to solve this problem for 1-2 months as part of my final individual project.

## What it does

This task was to develop an anomaly detection engine that gives the team an alert every time the data that are ingested each day are too low or too high compared to the usual traffic.

## How we built it

1. Collect the historical data from datalake
2. Research of the possible model
3. We initially though time-series problems could solve it easier
4. Used One-Class SVM Model that can detect anomalous number
5. Train and predict new number each day

## Challenge we ran into

I still often find some false positive cases, since the algorithm is quite sensitive with just a slight spike. But it is better than false negative cases.