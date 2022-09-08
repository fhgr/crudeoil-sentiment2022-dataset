# crudeoil-sentiment2022-dataset
This repository published the dataset used in the paper ``Combining affective and economic models with common knowledge to assess crude oil markets''.

## Contents
Description of the repository files

1. `evaluation.ipynb`: Python Jupyter Notebook outlining the evaluation (Dynamic Time Warping) outlined in the paper
2. `./dataset/news_headlines_and_sentiment_cogn2022.xlsx`: date, hashed headlines, source, and sentiment values for RavenPack, FinBERT, CrudeBERT and CrudeBERT+
3. `./dataset/crude_oil_price_and_sentiment_cogn2022.xlsx`: date, crude oil prices and sentiment values (raw and normalized)
4. `./dataset/headlines.xlsx`: example headline file used to create the full dataset
5. `./script/integrate-ravenpack-headlines.py`: Helper script used for extending the `dataset/news_headlines_and_sentiment_cogn2022.xlsx` file with the RavenPack headlines.


## How to obtain the RavenPack headlines
Please follow the following procedure to extend the `dataset/news_headlines_and_sentiment_cogn2022.xlsx` file with the RavenPack headlines:

 1. Log into [RavenPack](https://ravenpack.com/discovery/news_analytics_realtime/) and query for headlines published between 2012-01-01 and 2021-04-30,  with **Relevance** = **Highly Relevant** and **Novelty** = **Last Day** from its **crude oil** category.
 2. Save the query result as `headlines.xlsx` and copy it into the `dataset` directory.
 3. Change into the `dataset` directory and call `./../script/integrate-ravenpack-headlines.py` to create a new file that contains the headlines.
