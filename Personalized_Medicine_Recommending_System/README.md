# Medicine Recommendation System

## Overview
This project aims to build a medicine recommendation system based on textual descriptions and tags associated with medicines. The system leverages Natural Language Processing (NLP) techniques to analyze and process medicine descriptions, allowing for similarity calculations between medicines based on their descriptions. 

## Project Structure
- **`medicine.csv`**: This CSV file contains information about medicines including their names, reasons for use, and descriptions.
- **`medicine_recommendation.ipynb`**: This Jupyter Notebook contains the Python code for data preprocessing, text processing, and cosine similarity calculation to recommend similar medicines based on their descriptions.
- **`README.md`**: This file provides an overview of the project, its structure, and instructions on how to run and use the recommendation system.

## Requirements
- Python 3.x
- Libraries:
  - pandas
  - numpy
  - scikit-learn
  - nltk

## Setup
1. Clone the repository:
   ```
   git clone https://github.com/bhoomikamittal8/CodeClause_DataScienceIntern/tree/main/Personalized_Medicine_Recommending_System
   cd Personalized_Medicine_Recommending_System
   ```
   
2. Install the required libraries:
   ```
   pip install pandas numpy scikit-learn nltk
   ```
   
3. Run the Jupyter Notebook `medicine_recommendation.ipynb` to execute the recommendation system.

## Usage
1. Open the Jupyter Notebook `medicine_recommendation.ipynb`.
2. Execute each cell in the notebook to preprocess the data, compute cosine similarities between medicines, and define the recommendation function.
3. Use the `recommend(medicine_name)` function to get recommendations for a specific medicine based on its name.

## Functionality
- **Data Preprocessing**: The notebook reads data from `medicine.csv`, cleans and preprocesses text data (removing stopwords, stemming), and prepares it for similarity calculation.
  
- **Similarity Calculation**: Cosine similarity is used to determine how similar two medicines are based on their descriptions transformed into numerical vectors.

- **Recommendation**: The `recommend(medicine_name)` function takes a medicine name as input, retrieves its description, calculates similarities with other medicines, and recommends medicines with the highest similarity scores.

## Notes
- Ensure that `medicine.csv` is correctly formatted and contains the necessary fields (Drug_Name, Reason, Description) for the recommendation system to work properly.

## License
This project is licensed under the MIT License 


## Contact 📞

#### Feel free to email me or hit me up on [LinkedIn](https://www.linkedin.com/in/bhoomikamittal/)
