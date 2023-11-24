https://leetexplorer.onrender.com/

## Steps to run the code
1. Clone the repository
2. Run the prepare.py file to create the inverted index and the document frequency file
3. Run the app.py (flask --app app run) file to get the results for the queries

# LeetCode Question Search Tool

This project is a LeetCode question search tool that utilizes TF-IDF (Term Frequency-Inverse Document Frequency) and an inverted index to search for relevant questions based on keywords or tags. The search results are presented through a user-friendly web interface.

## Project Overview

The project consists of three main components:

1. **Data Preprocessing (`prepare.py`)**: The script processes the LeetCode question data, creating a vocabulary, calculating IDF values, and building an inverted index.

2. **Web Application (`app.py` and `index.html`)**: The Flask-based web application offers a user interface for conducting searches. It employs the processed data to calculate and display relevant question links.

## Getting Started

To use the LeetCode Question Search Tool, follow these steps:

1. **Data Preprocessing**:
   - Ensure you have the LeetCode question data saved in the `Qdata` folder.
   - Run `prepare.py` to preprocess the data, generate the vocabulary, IDF values, documents, and inverted index.
   - Processed data files are stored in the `tf-idf` folder.

2. **Web Application**:
   - Install the required Python packages by running `pip install flask flask_wtf`.
   - Run `app.py` to launch the Flask web application.
   - Access the application by navigating to `http://127.0.0.1:5000` in your web browser.

## Usage

1. Open the web application in your browser.
2. Input keywords or tags into the search box and click the "Search" button.
3. The application will display relevant question links, sorted by relevance score.

## Dependencies

- Python 3.x
- Flask
- Flask-WTF

## Project Structure

- `prepare.py`: Data preprocessing script
- `app.py`: Flask web application script
- `index.html`: HTML template for the web interface

- `tf-idf`: Processed data folder
  - `vocab.txt`: Vocabulary of terms and their IDF values
  - `idf-values.txt`: IDF values for each term
  - `documents.txt`: Processed documents
  - `inverted-index.txt`: Inverted index mapping terms to document indexes
