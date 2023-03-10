# Matching Algorithm
This script uses a combination of natural language processing techniques and nearest neighbor matching to identify possible matches between a list of missing taxpayer identification numbers (TINs) and a reference list of taxpayers with known TINs.

### Getting Started
To use this script, you will need to provide a list of of names in an Excel file, along with the name of the sheet containing the data. You will also need to provide a reference list of names in another Excel file, along with the name of the sheet containing the data.

### Prerequisites
This script requires the following Python libraries to be installed:

pandas
numpy
scikit-learn

### How it works
The script uses the cosine similarity between two vectors to calculate the similarity between two strings. This allows it to identify matches between strings that are not exact matches.

The script also uses the TfidfVectorizer class from scikit-learn to convert the names in the reference list of taxpayers into feature vectors. It then uses the NearestNeighbors class from scikit-learn to identify the nearest neighbor to each unique name in the set of missing TINs.

The script outputs a DataFrame containing the matches, along with a confidence score based on the cosine similarity between the two strings.

### How to use it
To use the script, simply download the script and install the required libraries. Then, update the file paths in the script to point to your input files.

You can also adjust the n parameter in the ngrams function to control the length of the n-grams used in the feature vectorization process.

### License
This project is licensed under the MIT License.
