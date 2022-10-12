## Introduction
----------------------
This data set contains simulated data offerd by Starbucks of how people make purchasing decisions and how those decisions are influenced by promotional offers.
Each person in the simulation has some hidden traits that influence their purchasing patterns and are associated with their observable traits. People produce various events, including receiving offers, opening offers, and making purchases.
As a simplification, there are no explicit products to track. Only the amounts of each transaction or offer are recorded.
There are three types of offers that can be sent: buy-one-get-one (BOGO), discount, and informational. In a BOGO offer, a user needs to spend a certain amount to get a reward equal to that threshold amount. In a discount, a user gains a reward equal to a fraction of the amount spent. In an informational offer, there is no reward, but neither is there a requisite amount that the user is expected to spend. Offers can be delivered via multiple channels.
The basic task is to use the data to identify which groups of people are most responsive to each type of offer, and how best to present each type of offer.

We analyzed thsi dataset and tried to find interesting observations using data analytics technics.

## Dataset
-------------------
The data is contained in three files:
	• portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
	• profile.json - demographic data for each customer
	• transcript.json - records for transactions, offers received, offers viewed, and offers completed
Here is the schema and explanation of each variable in the files:
1. portfolio.json
	Rewards program users (17000 users x 5 fields)
	• id (string) - offer id
	• offer_type (string) - type of offer ie BOGO, discount, informational
	• difficulty (int) - minimum required spend to complete an offer
	• reward (int) - reward given for completing an offer
	• duration (int) - time for offer to be open, in days
	• channels (list of strings)
2. profile.json
	Offers sent during 30-day test period (10 offers x 6 fields)
	• age (int) - age of the customer
	• became_member_on (int) - date when customer created an app account
	• gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
	• id (str) - customer id
	• income (float) - customer's income
3. transcript.json
	Event log (306648 events x 4 fields)
	• event (str) - record description (ie transaction, offer received, offer viewed, etc.)
	• person (str) - customer id
	• time (int) - time in hours since start of test. The data begins at time t=0
	• value - (dict of strings) - either an offer id or transaction amount depending on the record


## Links
---------------------
https://medium.com/........

## Attachments
----------------------
- portfolio.json
- profile.json
- transcript.json
- Starbucks_Capstone_notebook.ipynb - a Jupyter notebook showing data set loading, cleaning, investigation 

## Acknowledgements:
----------------------
The data was provided by Starbucks



For more details, please refer to ....