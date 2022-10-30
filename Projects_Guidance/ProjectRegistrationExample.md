# Project registration example

Project title: Political strength in Online Social Impact

Names and email addresses of group members:  
Student 1, email1@domain.com (X major)  
Student 2, email2@domain.com (Y major)  
Student 3, email3@domain.com (Z major)  
Student 4, email4@domain.com (W major)

Research question(s):  
We aim to test the hypothesis of the role of strength in social impact as hypothesized by Social Impact Theory. We will study how the strength of a source on Twitter influences the aggregated impact it has on its followers. To do so, we will focus on US accounts of current and former members of congress and analyze their timelines, measuring strength as a comparison between two groups: current members as strong sources and past members as weaker sources. We will test the following hypotheses:  

1. The mean number of retweets per tweet of twitter accounts of US politicians grows as a power of number of followers (replication of exercise).  

2. The mean number of retweets per tweet of twitter accounts of current members of congress is higher than former members of congress.  

3. The coefficient of the relationship between mean number of retweets per tweet and the number of followers is higher for current the twitter accounts of current members of congress than for former members of congress (multiplicative effect).

Planned data retrieval and analysis to address the questions

We plan the following steps

1. Based on an existing dataset (https://osf.io/mqhgp/), retrieve twitter user profile data and remove from the analysis any accounts that are set to private, have less than 100 followers, wrote less than 100 tweets, or had their last tweet more than a month ago.

2. Retrieve tweets posted in the last year by each of the remaining accounts.

3. Clean tweets by removing retweets, replies, and tweets younger than two days old.

4. Record the impact of each account as the mean number of retweets of their tweets. Produce a data frame per user with a column for the mean number of retweets, a second column for the number of followers, and a third with a code of whether they are current or former congress members.

5. Fit linear regression models to test each of the hypotheses. We will apply permutation tests to estimate the p-value of the hypotheses versus their corresponding null hypothesis and we will use bootstrapping to calculate the confidence intervals around the coefficients we are interested in.

