## Notes
What's Implemented: Exploratory Data Analysis (EDA); Matrix Factorization; Multi-Objective Recommender System (MORS); Collaborative Filtering; Content-based Filtering; Neural Collaborative Filtering (NCF)
Potential Improvements:
Time Used:
Study Notes:

## OTTO – Multi-Objective Recommender System
(Kaggle Link)[https://www.kaggle.com/competitions/otto-recommender-system/overview]
Build a recommender system based on real-world e-commerce sessions

### Description
Goal of the Competition
The goal of this competition is to predict e-commerce clicks, cart additions, and orders. You'll build a multi-objective recommender system based on previous events in a user session.

Your work will help improve the shopping experience for everyone involved. Customers will receive more tailored recommendations while online retailers may increase their sales.

Context
Online shoppers have their pick of millions of products from large retailers. While such variety may be impressive, having so many options to explore can be overwhelming, resulting in shoppers leaving with empty carts. This neither benefits shoppers seeking to make a purchase nor retailers that missed out on sales. This is one reason online retailers rely on recommender systems to guide shoppers to products that best match their interests and motivations. Using data science to enhance retailers' ability to predict which products each customer actually wants to see, add to their cart, and order at any given moment of their visit in real-time could improve your customer experience the next time you shop online with your favorite retailer.

Current recommender systems consist of various models with different approaches, ranging from simple matrix factorization to a transformer-type deep neural network. However, no single model exists that can simultaneously optimize multiple objectives. In this competition, you’ll build a single entry to predict click-through, add-to-cart, and conversion rates based on previous same-session events.

With more than 10 million products from over 19,000 brands, OTTO is the largest German online shop. OTTO is a member of the Hamburg-based, multi-national Otto Group, which also subsidizes Crate & Barrel (USA) and 3 Suisses (France).

Your work will help online retailers select more relevant items from a vast range to recommend to their customers based on their real-time behavior. Improving recommendations will ensure navigating through seemingly endless options is more effortless and engaging for shoppers.

### Dataset Description
The goal of this competition is to predict e-commerce clicks, cart additions, and orders. You'll build a multi-objective recommender system based on previous events in a user session.

The training data contains full e-commerce session information. For each session in the test data, your task it to predict the aid values for each session type thats occur after the last timestamp ts in the test session. In other words, the test data contains sessions truncated by timestamp, and you are to predict what occurs after the point of truncation.

For additional background, please see the published OTTO Recommender Systems Dataset GitHub.

Files
train.jsonl - the training data, which contains full session data
session - the unique session id
events - the time ordered sequence of events in the session
aid - the article id (product code) of the associated event
ts - the Unix timestamp of the event
type - the event type, i.e., whether a product was clicked, added to the user's cart, or ordered during the session
test.jsonl - the test data, which contains truncated session data
your task is to predict the next aid clicked after the session truncation, as well as the the remaining aids that are added to carts and orders; you may predict up to 20 values for each session type
sample_submission.csv - a sample submission file in the correct format