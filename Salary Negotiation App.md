Salary Negotiation App
========================================================
author: Peter Caya
date: 5/12/2017
autosize: true


The Issue We Approach
========================================================

Companies keep or buy data so they know exactly how much a role is "worth".  
Applicants, especially graduates are not able to match this research.  The result is that people that are establishing their careers are often at a loss as to:

1. How good the proposed salary actually is.
2. How the salaries compare across cities.


What We Should Offer
========================================================

A simple app that does the following:

1. Takes a list of parameters (city, job title, years experience, college major).
2. Generate summary statistics on salary for a role based on open and proprietary data.

Potential later additions to compare:

1. Salary across cities.
2. Similar job types (for instance, statistical analyst and business analyst).



Data Sources
========================================================

Prepackaged Data:

* [The Bureau of Labor Statistics](https://www.bls.gov/)
* [US Census.gov](https://www.census.gov/data.html)
* [Quandl](https://www.quandl.com/)
* [Federal Reserve Bank of St. Louis Economic Research](https://fred.stlouisfed.org/)

Data to be Processed:

* [indeed.com API](https://github.com/indeedlabs/indeed-python)
* [Glassdoor API](https://www.glassdoor.com/developer/index.htm)
* [LinkedIn API](https://developer.linkedin.com/)



Data Pipeline
========================================================

## Data Processing:

1. Prepacked data can be easily downloaded and processed.
2. Information from the APIs will have to be processed after being downloaded.
  * For instance, if we want to get a metric on the phrase 
  1 to 3 years of experience" we will have to  process the data from job descriptions.
  

## Data Storage:

Data can be stored using SQLite database which will act as the "back-end" of the app.


<!-- ## Accessing the Data: -->

<!-- A user will enter the type of job, years of experience, and other factors.   -->

<!-- Data will be returned from the database, and then some algorithm will be used on the filtered data to estimate a salary range. -->


Deploying the App
========================================================

To start, Shiny R can be used as the front end.  As we more is expected of the app, it can be expanded as a more standalone system.

Advantages of R Shiny:

1. Quick and simple to create and share mimimal working example.
2. Integrated in statstical programming environment.
3. Flexible and appealing interface:  [Example](https://shiny.rstudio.com/gallery/superzip-example.html)



Looking Forward:  Traffic and Money
========================================================

* Google Ads
* Amazon affiliate
* Redirecting to Indeed.com/Glassdoor (Have not research this path).

