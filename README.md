## Project summary:
----------------
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

This project uses python to read the contents of the csv files and then stores the data in Apache Cassandra databases. 

## How it works:
-------------
The project contains two files:

**event_datafile_new.csv:** This file contains the data that must extracted and analyzed.

**Project_1B_Project_Template.ipynb:**
This file contains the entire code.
The data is read using a csv reader object and inserted directly into the Cassandra tables. They are designed by first constructing queries based on the specific questions that the analytics team wishes to answer. We then read the entire csv file and store the relevant data in the table.
We then run each queries to answer the desired questions and observe a limited number of rows resulting from our queries.
Once we are satisfied with the output, we drop the tables and shutdown our session.

## How to use the scripts:
-----------------------
Simply run the Jupyter notebook cells.
