# Starbucks-Capstone-Challenge

### Table of Contents

1. [Project Overview](#overview)
2. [Installation](#installation)
3. [File Descriptions](#files)
4. [Instructions](#instructions)
5. [Results](#results)
6. [Licensing, Authors, and Acknowledgements](#licensing)

## Project Overview <a name="overview"></a>
The goal of of this project is to develop recommendation engine to determine what offer you should send to each customer. We plan to build two systems:
1. Simple System for new customers which we do not have much information about them
2. Target-based System for existing customers leveraging on the customer demographics and transactional data given


## Installation <a name="installation"></a>
The code should run with no issues using Python versions 3.*, with libraries of numpy, pandas, math, json, date, matplotlib and seaborn.

## File Descriptions <a name="files"></a>
The data is contained in three files:
- portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
- profile.json - demographic data for each customer
- transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

portfolio.json

- id (string) - offer id
- offer_type (string) - type of offer ie BOGO, discount, informational
- difficulty (int) - minimum required spend to complete an offer
- reward (int) - reward given for completing an offer
- duration (int) - time for offer to be open, in days
- channels (list of strings)

profile.json

- age (int) - age of the customer
- became_member_on (int) - date when customer created an app account
- gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
- id (str) - customer id
- income (float) - customer's income

transcript.json

- event (str) - record description (ie transaction, offer received, offer viewed, etc.)
- person (str) - customer id
- time (int) - time in hours since start of test. The data begins at time t=0
- value - (dict of strings) - either an offer id or transaction amount depending on the record

## Instructions <a name="instructions"></a>

The following files are in this GitHub repository:
- Starbucks_Capstone_notebook.ipynb: the Jupyter Notebook for my work
- Raw data provided by Starbucks/ Udacity (except for transcript.jason - which I included here a zip version instead due to file size limitation

## Results <a name="results"></a>
The main findings of the code can be found at the post available [here](https://medium.com/@chriswongpy/sending-starbucks-offers-more-effectively-a359bceb3228)

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

credit to Starbucks and Udacity for providing the data for this project.  
