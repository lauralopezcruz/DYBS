<img width="400" alt="portfolio_view" src="https://cdn.pixabay.com/photo/2019/11/03/16/29/woman-4599055_1280.png">

# A Book Recommendation System to
# Decolonize your Bookshelf


> I combine two collaborative filtering algorithms, a ratings-based algorithm and a content-based one, to create an app that takes as input a book and recommends similar books written by authors of color.


**Outline of Jupyter notebooks:**

1. **Labelling:** I use book tags from the Kaggle dataset to label some authors, then I scrape a list of POC authors from Goodreads.

2. **Ratings_similarity:** I create a ratings-based book similarity matrix using ratings data from Goodreads. This code is not mine.

3. **Scraping_summaries:**  Here I have short script to scrape all (but 45) book summaries from Goodreads.com. The last 45 books did not have summaries.

4. **Topic_Modeling:** I do topic modeling on the summaries. I use CorEx to get topics, SpaCy for preprocessing the text.

5. **App:**: I build a function that takes as input a book id, a number k, and a percentage n, and outputs k similar books where content is weighed by n% and ratings by 100-n%.
