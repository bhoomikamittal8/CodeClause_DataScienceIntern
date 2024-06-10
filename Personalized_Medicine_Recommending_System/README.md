# Personalized_Medicine_Recommending_System

code performs the following tasks to create a content-based medicine recommendation system:

**Data Preparation:**

The code begins by importing essential libraries, such as NumPy, Pandas, NLTK, Scikit-Learn, and others.
It loads a dataset containing medicine information from a CSV file named 'medicine.csv' into a Pandas DataFrame.
Data cleaning is performed to handle missing values, duplicate rows, and unnecessary spaces in the dataset.

**Text Data Preprocessing:**

The 'Description' and 'Reason' columns are tokenized, splitting their text into lists of individual words.
These two columns are combined into a new 'tags' column, which serves as the basis for similarity calculations.
Text data in the 'tags' column is converted to lowercase for consistency.

**Text Normalization:**

The Porter Stemmer from NLTK is applied to the 'tags' column to reduce words to their root forms. This process helps improve the accuracy of similarity calculations.

**Vectorization:**

The CountVectorizer from Scikit-Learn is used to transform the preprocessed 'tags' column into a document-term matrix. This matrix represents the text data as numerical vectors.
The CountVectorizer also removes English stop words and limits the feature set to the top 5000 most frequent words.

**Cosine Similarity Calculation:**

Cosine similarity scores are computed for all pairs of medicine descriptions using the document-term matrix. The result is a similarity matrix that quantifies the similarity between medicines based on their descriptions and reasons for use.

**Recommendation Function:**

A function named recommend is defined to provide medicine recommendations based on user input.
The function takes the name of a medicine as input and identifies the most similar medicines based on cosine similarity scores.
It returns the top 5 medicines that are most similar to the input medicine.

**Model Saving:**

The code uses the pickle library to save two important components of the recommendation system:
The processed dataset with normalized text information is saved as 'medicine_dict.pkl'.
The similarity matrix, which contains cosine similarity scores, is saved as 'similarity.pkl'. These saved components can be loaded later for reuse.


In summary, this code creates a content-based recommendation system for medicines, allowing users to find similar medicines based on descriptions and reasons for use. The system leverages natural language processing techniques to process and analyze text data, making it a valuable tool for healthcare professionals and patients looking for alternative medicines with similar characteristics.
