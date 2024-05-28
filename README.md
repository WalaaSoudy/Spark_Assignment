
# Wikimedia Page View Statistics Analysis

## Introduction

This project involves analyzing the page view statistics of Wikimedia projects using Apache Spark. The dataset contains statistics for Wikimedia pages between 0-1 am on Jan 1, 2016. Each line of the dataset includes the project code, page title, page hits, and page size.

## Dataset

The dataset can be downloaded from [here](https://dumps.wikimedia.org/other/pageviews/2016/2016-01/pageviews-20160101-000000.gz).

The schema for the dataset is as follows:
- **Project code**: The project identifier for each page.
- **Page title**: A string containing the title of the page.
- **Page hits**: Number of requests in the specific hour.
- **Page size**: Size of the page.

## Queries

1. Compute the minimum, maximum, and average page size.
2. Determine the number of page titles that start with the article “The”. Also, find out how many of these titles are not part of the English project (project code “en”).
3. Determine the number of unique terms appearing in the page titles. Normalize terms by lowercasing and removing non-alphanumeric characters.
4. Extract each title and the number of times it was repeated.
5. Combine data of pages with the same title and save each pair of pages data.

## Implementation

The application is implemented using Apache Spark in two paradigms:
- MapReduce paradigm
- Spark loops paradigm

