# Capstone-Project

## Overview

This repository is to report the Starbuck's Capstone Challenge of the Data Scientist Nanodegree in Udacity. 
The dataset is from the program that creates the data simulates how people make purchasing decisions and how those decisions are influenced by promotional offers. 
The goal of the project is to make a recommendation engine that recommends Starbucks which offer should be sent to a particular customer.

We are interested in answering **Which offer should be sent to a particular customer to let the customer buy more?**

An article of the project can be found in [here](https://medium.com/@juliacaria/starbucks-capstone-challenge-f7cd5523df94?sk=eb2f2d044e625eef8468acd555d7f17e). 

## Repository Contents


The data is contained in three files:

-   `portfolio.json`  - containing offer ids and meta data about each offer (duration, type, etc.)
-   `profile.json`  - demographic data for each customer
-   `transcript.json`  - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

`portfolio.json`

-   id (string) - offer id
-   offer_type (string) - the type of offer ie BOGO, discount, informational
-   difficulty (int) - the minimum required to spend to complete an offer
-   reward (int) - the reward is given for completing an offer
-   duration (int) - time for the offer to be open, in days
-   channels (list of strings)

`profile.json`

-   age (int) - age of the customer
-   became_member_on (int) - the date when customer created an app account
-   gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
-   id (str) - customer id
-   income (float) - customer's income

`transcript.json`

-   event (str) - record description (ie transaction, offer received, offer viewed, etc.)
-   person (str) - customer id
-   time (int) - time in hours since the start of the test. The data begins at time t=0
-   value - (dict of strings) - either an offer id or transaction amount depending on the record
