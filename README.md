# Project 2 - Data Ingestion & Analysis

***Project.py*** is the script to call the remote api exactly every minute, writing the data to a sql database stored in Amazon RDS.

***Data Screenshot*** is a screenshot of the data table (apidata) produced from the project.py script. The screenshot is large, so you might have to scroll to the right to see the "time" column.
  
  The purpose of this project was to familiarize myself with API's and how to write the data to remote databases. My process for this project was to first figure out the script and how to pull from the api and push its data to a sql table. To accomplish this, I created a new database in AWS RDS, then used phpmyadmin to set up columns in a new table. Pulling from the api exactly every minute was tricky as the program's runtime "drifts" the pull request time, but I found the [Twisted python package](https://docs.twistedmatrix.com/en/stable/api/twisted.internet.html), which helped me pull and push the api data to the table exactly every minute. While this is a simple project, interacting and familiarizing myself with API's, Amazon's web services, and how to work with these tools in python served as a great introduction to higher level data science.
