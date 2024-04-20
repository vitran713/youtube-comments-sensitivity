This Jupyter notebook is designed to extract and analyze YouTube video comments using the YouTube Data API. Below is a summary of the functionalities implemented in the notebook:

YouTube API Integration: I've set up a function to connect to the YouTube API and fetch comments from specified video IDs. This function handles the retrieval of comments across multiple videos and compiles them into a single list. The comments are then stored in a pandas DataFrame and outputted to a CSV file for further analysis.

Data Loading and Text Analysis: After gathering the comments, I load the data from the CSV file into a DataFrame. I clean the data by ensuring there are no missing values and that all entries are strings. I then utilize the Natural Language Toolkit (nltk) to tokenize the text and apply basic natural language processing techniques. This includes observing the distribution of word frequencies and applying Zipf’s Law to understand the prominence of certain words in the comments.

Text Preprocessing and Word Frequency Calculation: I continue with advanced text preprocessing steps including converting all text to lowercase, removing punctuation, and filtering out stopwords to focus on more meaningful words. Using the processed text, I calculate the frequency of each word and identify the most common words used across the comments. These findings are saved to another CSV file and can be used for detailed textual analysis or feature selection.

Attribute Selection: Lastly, I've incorporated an interactive segment where users can select specific attributes or words from the analyzed data. This feature is designed to assist in narrowing down the analysis to particular areas of interest based on the frequency and relevance of the words.
