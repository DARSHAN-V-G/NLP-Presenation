# NLP Presentation - Keyword Extraction

This repository contains a demonstration of Natural Language Processing (NLP) techniques used to extract keywords from a PDF document. The project compares three popular keyword extraction algorithms to show different approaches to identifying the most relevant terms and phrases in a text.

## Features

- **PDF Text Extraction**: Uses `pdfminer` to automatically parse and extract raw text from PDF files.
- **Text Preprocessing**: Cleans the text using `nltk` by lowercasing, tokenizing, and removing punctuation and stopwords.
- **Multiple Extraction Algorithms**:
  - **TF-IDF (Term Frequency-Inverse Document Frequency)**: A statistical measure evaluating how relevant a word is to a document in a collection.
  - **RAKE (Rapid Automatic Keyword Extraction)**: An unsupervised, domain-independent method that determines key phrases by analyzing word co-occurrences.
  - **KeyBERT**: A minimal and easy-to-use keyword extraction technique that leverages BERT embeddings to find the most similar keywords to a document.

## Repository Structure

```
NLP-Presenation/
├── .gitignore
└── keyword_extraction/
    ├── app.py          # Main Python script for extraction
    └── sena3.pdf       # Example IEEE PDF document used for extraction
```

## Prerequisites and Dependencies

To run this project, you will need Python 3 installed along with several external libraries. You can install the required packages using pip:

```bash
pip install pdfminer.six nltk scikit-learn rake-nltk keybert
```

*Note: The script will automatically download the necessary NLTK corpora (`punkt`, `punkt_tab`, and `stopwords`) upon its first run if they are not already installed.*

## Usage

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/Dhaarun-Abhimanyu/NLP-Presenation.git
   cd NLP-Presenation/keyword_extraction
   ```

2. Ensure your target PDF is named `sena3.pdf` and placed in the `keyword_extraction` directory. (If you want to use a different PDF, update the `pdf_file` variable in `app.py`).

3. Run the script:
   ```bash
   python app.py
   ```

4. The script will output the extraction progress and print the top keywords identified by each of the three algorithms to your terminal.

## Contributors

- [@Dhaarun-Abhimanyu](https://github.com/Dhaarun-Abhimanyu)
