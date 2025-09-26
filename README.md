# Masters-Thesis-code
#Explanation of the steps I used 

Step-by-Step Explanation of the Code

- Data Collection: The code begins by using the PRAW library to connect to Reddit’s API and fetch recent posts from subreddits such as entrepreneur, startups, and passive_income. Posts are filtered to retain only those containing relevant business-related keywords, such as SaaS, income, or startup.

- Preprocessing: The collected text data is cleaned by removing URLs and special characters, converting all text to lowercase, and tokenizing it into individual words. Each token is lemmatized (e.g., “running” becomes “run”) and common stopwords (like “the,” “a,” “is”) are removed to reduce noise and improve analysis.

- Vectorization: The cleaned text is transformed into numerical representations suitable for machine learning models. TF-IDF (Term Frequency–Inverse Document Frequency) is applied to measure the importance of each word relative to its occurrence across all documents.

- Analytics: The vectorized data is then analyzed using multiple techniques:

- Topic modeling with LDA and NMF identifies underlying themes in the discussions.

- Clustering with K-Means groups posts with similar content.

- Trend analysis highlights the most frequent terms over time, showing how topics evolve.

- Outcome: Overall, the code provides a data-driven analysis of Reddit discussions on entrepreneurship. By collecting, cleaning, and processing posts, it automatically identifies key themes such as passive income, SaaS development, and startup strategies, offering a clear overview of the main topics in these online communities.
