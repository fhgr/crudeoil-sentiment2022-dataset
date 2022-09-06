# crudeoil-sentiment2022-dataset
Hashed RavenPack headlines, the corresponding sentiment values and crude oil prices from 2004-2021


Please follow the following procedure to recreate the headlines:

 1. Log into [RavenPack](https://ravenpack.com) and query for headlines published between 2012-01-01 and 2021-04-30, and labeled as **highly relevant** to its **crude oil** categories.
 2. Save the query result as `headlines.xlsx` and copy it together with the `headlines_with_sentiment_scores_cogn2022.xlsx` file to your working directory.
 3. Calling `./script/integrate-ravenpack-headlines.py` will create a new file that contains the headlines.
