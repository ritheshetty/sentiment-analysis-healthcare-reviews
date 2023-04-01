# sentiment-analysis-healthcare-reviews
Performed a sentiment analysis on healthcare reviews to gauge the perception of the healthcare system in that region using 3 different models: Naive Bayes, SVM and DistilBERT.
This is a component in a larger healthcare analytics tool where we generate a perception score on a county-by-county basis in the United States.


Dataset:

Since there was no freely available dataset, it was necessary to gather the data by scraping the reviews from the Yelp API. Using the free API, 5000+ physician and clinic reviews were collected and pre-processed to get them model ready.
I noticed that the reviews were highly biased to 1 and 5 stars, which would skew the model. Hence the reviews were subsampled to create a more balanced dataset, included in "BalancedReviews3Class.csv".

Model exploration:

Several different models were explored, such as Naive Bayes, Support Vector Machine, BERT and DistilBERT. Of course, DistilBERT produced state-of-the-art performance with a validation accuracy of 97% and ended up being the model of choice for the sentiment analysis task at hand.

Performance benchmarks:

A detailed report is included to highlight performance benchmarks and processes involved.


The files included are Jupyter notebooks. 
