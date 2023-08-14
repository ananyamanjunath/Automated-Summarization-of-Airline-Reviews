# Airline Reviews Summarization using BART

This project involves generating concise summaries for airline reviews using the BART (Bidirectional and Auto-Regressive Transformers) model. The goal is to automatically generate summaries that capture the essence of the reviews in a succinct manner. Here's an overview of the project:

## Data Preprocessing

The project begins by loading the airline reviews dataset and selecting the first 20 datapoints for analysis. The reviews are then preprocessed using spaCy's pre-trained model to tokenize the text and remove stopwords. The preprocessed reviews are stored in the 'Processed_Review' column.

## Model Initialization

The BART model and tokenizer are initialized for sequence-to-sequence language modeling. The BART model is pre-trained on a large corpus and can generate coherent and contextually relevant summaries.

## Summary Generation

A function is defined to generate concise summaries for the preprocessed reviews using the initialized BART model. The function encodes the input text, generates summary IDs, and decodes the summary using the tokenizer. Parameters such as maximum and minimum length, length penalty, and number of beams are specified to control the summary generation process.

## Summarizing Reviews

The project concludes by generating summaries for the first 20 preprocessed reviews using the BART model. Each review is summarized, and the corresponding summary is printed.

## Installation

Before running the provided code, make sure you have the required dependencies installed:

-   Python 3
-   pandas
-   spaCy
-   transformers (Hugging Face)

You can install these dependencies using the following command:

```bash
pip install pandas spacy transformers
```

## Usage

Follow these steps to use the code:

1.  Clone this repository to your local machine:

```bash
git clone https://github.com/ananyamanjunath/Automated-Summarization-of-Airline-Reviews.git
```

2.  Download the airline reviews dataset (`Airline_Reviews.csv`) and place it in the appropriate directory of the project.
    
3.  Launch Jupyter Notebook and open the `airline_reviews_summarization.ipynb` notebook.
    
4.  Execute the code cells in the notebook sequentially to generate concise summaries for the airline reviews. The notebook provides detailed explanations of each step.
    
5.  Explore the generated summaries and gain insights from the review summarization.
    

## Acknowledgments

This project draws inspiration from various resources on text summarization and transformer-based language models. The use of spaCy and Hugging Face's Transformers library enhances the efficiency and effectiveness of the summarization process.
