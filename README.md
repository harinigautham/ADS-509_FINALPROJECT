# ADS-509_FINALPROJECT

The goal of this project is to perform text classification and topic modeling on extracted airline reviews. In order to acquire this data, the Playwright library is utilized to scrape reviews from TripAdvisor, a popular travel website. The initial web scraper is written to extract all airlines reviewed on TripAdvisor, along with the total reviews posted for each one. This information allows us to gain a better understanding of data availability. Skytrax was scraped as well, due to the regional filters provided by the website. These regions are incorporated in the dataset as classes for extracted reviews. Regional differences might influence the textual information present in reviews, potentially resulting in more accurate text classification models. One airline is chosen to represent each of the 10 distinct regions. TripAdvisor is scraped again, gathering 100 reviews/titles for each of the ten airlines, along with their 5-star rating. Descriptive Statistics are calculated on each of these airlines, calculating the total token count, amount of unique tokens, character count, and lexical diversity for each one.

- airline_reviews.json: contains the TripAdvisor information extracted in the initial web scraper
- tokenized_reviews.json: contains the final dataset used for modeling
- data_extraction_cleaning.ipynb: contains code for the webscrapers built, data cleaning, and descriptive statistics
- topic_modeling_classification.ipynb: contains code for the topic models and text classification models built
