# What’s the cost of bad press? The impact of social media chatter on share prices.

## Research question
Do social media postings impact the value of a company, and to what extent? I will explore the causal impact of adverse social media exposure on a company’s value as indicated by share prices. 


## Motivation 
Social media is one of the most common avenues for people to receive information; however, its impacts beyond simple entertainment are still largely unknown.  Here, I wish to explore how social media impacts publicly traded companies, which has been only minimally explored academically.  This project serves to expand academic understanding of the influence of social media, as well as providing a new economic tool for assessing and predicting share prices.


## Expected contribution 
By identifying a causal relationship between social media postings and share price, I seek to contribute to the small body of research on how press influences price.  Furthermore, by quantifying the causal effect of negative social media on share prices, I will offer a useful predictive tool for assessing the damage done by negative social media exposure that can be used for analysis or prediction. 


## Preliminary literature context
Using Social Media to Identify the Effects of Congressional Viewpoints on Asset Prices
Teti, E., Dallocchio, M., & Aniasi, A. (2019). The relationship between twitter and stock prices. Evidence from the US technology industry. Technological Forecasting and Social Change, 149, 119747. https://doi.org/10.1016/j.techfore.2019.119747

Nishimura, Y., & Sun, B. (2025). Impacts of Donald Trump's tweets on volatilities in the European stock markets. Finance Research Letters, 72, 106491. https://doi.org/10.1016/j.frl.2024.106491

Cam, H., Cam, A. V., Demirel, U., & Ahmed, S. (2024). Sentiment analysis of financial Twitter posts on Twitter with the machine learning classifiers. Heliyon, 10(1), e23784. https://doi.org/10.1016/j.heliyon.2023.e23784

Das, S., Behera, R. K., Kumar, M., & Rath, S. K. (2018). Real-Time Sentiment Analysis of Twitter Streaming data for Stock Prediction. Procedia Computer Science, 132, 956-964. https://doi.org/10.1016/j.procs.2018.05.111

## Data sources and feasibility
Data will come from Bloomberg and through the APIs for Twitter and Instagram as follows:
- Share price: Panel data on share price by company from Bloomberg
Share price: Panel data on share price by company from Bloomberg
Social media sentiment: Bloomberg Intelligence
Social media sentiment analysis: Will create a tool to use natural language processing to generate a sentiment score with distribution U[-1,1]


## Initial empirical strategy idea
Using negative sentiment as “treatment,” evaluate the causal effect of treatment against days with neutral press as controls, then average across all companies.  Only posts from high-profile accounts will be used initially from a short list of individuals/organizations.  To address confounding from other company actions, such as earnings releases, I will ignore share performance around earnings calls.  Also, I will experiment with lags from 1 hour to 1 week after a post to try to address possible confounding from other market forces or social media trends. 


## Anticipated challenges
Isolation of the specific causal effect of social media (as opposed to just news) is difficult, but has been done in the past.  I will be iterating on previous approaches in published academic literature.  


Building the full software pipeline needed for this will be a stretch for my engineering skills.  However, I believe that I can do it, and it will be a good learning experience.  It will also be difficult to obtain reproducible results because of the LLM usage requirement to generate a sentiment metric.  


I will also need to avoid scope creep.  It is easy to let this encompass all stocks, all tweets/posts, etc.  To avoid that, I will cap the number of stocks looked at to 50, and will initially explore the posts of 10-15 high-profile individuals in finance and/or politics (e.g., Jamie Dimon, Ray Dallio, etc.). 
