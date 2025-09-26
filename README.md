# Masters-Thesis-code
Code file for thesis 

Step-by-Step explanation:
First, in the Data Collection phase, the code uses the Praw library to connect to Reddit's API. It fetches recent posts from subreddits like "entrepreneur," "startups," and "passive_income." The collected posts are then filtered to ensure they contain relevant business-related keywords such as 'saas', 'income', or 'startup'.
Next, the Preprocessing stage cleans the raw text data. This involves removing URLs and special characters, converting the text to lowercase, and then tokenizing it (splitting it into individual words). Each word is lemmatized, meaning it's reduced to its root form (e.g., "running" becomes "run"), and common "stopwords" (like "the," "a," "is") are removed to reduce noise.
In the Vectorization step, the cleaned text is converted into numerical representations that machine learning models can process. The code uses TF-IDF, a method that measures the importance of a word in a document relative to its frequency across all documents.
Finally, the Analytics phase applies several techniques to the vectorized data. Topic modeling algorithms like LDA and NMF are used to discover underlying themes in the discussions. The posts are also grouped into clusters of similar content using K-Means. The script concludes by performing a simple trend analysis, identifying the most frequent terms over time to see how topics evolve.
Overall, this code successfully analyzes Reddit discussions on entrepreneurship. By collecting, cleaning, and processing posts, it uses machine learning to automatically identify key themes like "passive income," "SaaS development," and "startup strategies." The result is a clear, data-driven overview of the main topics being discussed in these online communities.
