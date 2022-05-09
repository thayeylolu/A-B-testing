# A-B-testing
An A/B testing using Statistical tools in R.

## Introduction

In this Project, I will work with the AdSmartABdata data I found on Kaggle. I intend to run a case study where A/B testing is applied on the click through rate. The primary aim is to compare user interactions with the bio questionnaire to determine which interaction statistically improves CTR .

## Data 
The Data is available on Kaggle here is the [link](https://www.kaggle.com/datasets/osuolaleemmanuel/ad-ab-testing).

**The Data Columns**

- auction_id: the unique id of the online user who has been presented the BIO questionnaire. • experiment: which group the user belongs to - control or exposed.
– control: users who have been shown a dummy ad
– exposed: users who have been shown a creative, an online interactive ad, with the SmartAd
brand.
- date: the date in YYYY-MM-DD format
- hour: the hour of the day in HH format.
- device_make: the name of the type of device the user has e.g. Samsung
- platform_os: the id of the OS the user has.
- browser: the name of the browser the user uses to see the BIO questionnaire. 
     - yes: 1 if the user chooses the “Yes” radio button for the BIO questionnaire.
     - no: 1 if the user chooses the “No” radio button for the BIO questionnaire.

## Questions
The following Statisitcal questions are asked : 

**1. A/B testing Comparing CTR (Click Through Rate) **

Does the CTR of exposed perform better than control when

 - Users click on the BIO questionnaire?

 - Users fill the BIO questionnaire?

**2. Causality - Blocking**

I will address these problems by blocking on a variable

 - Does clicking(answering) the bio questionnaire of the smart ad or dummy ad (yes or no = 1) cause an improvement in user engagement?

 - Does engaging (yes = 1) with the bio questionnaire of the smart ad(exposed) or dummy ad(control) ad result in an improvement in user engagement?


## Statisitcal Result Summary
**A/B testing Comparing CTR**
The Proportion test on the CTR for the two treatments **exposed** and **control** (_alpha : 0.05_) :
- **Users click on the BIO questionnaire**: Exposed performed better than control with a CTR of 16.5% and 14.5% respectively.
- **Users fill the BIO questionnaire**: Exposed performed better than control with a CTR of 7.75% and 6.5% respectively.

**Causality - Blocking** (_In progress_)

