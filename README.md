# What is LangExtract

LangExtract is a Python library that uses LLMs to extract structured information from unstructured text documents based on user-defined instructions. It processes materials such as clinical notes or reports, identifying and organizing key details while ensuring the extracted data corresponds to the source text.

# Sentiment Extraction with LangExtract

This repository demonstrates how to use the `LangExtract` library for extracting sentiment phrases and their attributes from text. The notebook walks through the process of setting up the environment, defining rules for extraction, and using the `LangExtract` library for analysis.

## Features

- **Sentiment Phrase Extraction**: Extracts sentiment phrases directly from the text without paraphrasing.
- **Sentiment Attributes**: Categorizes sentiments (e.g., positive, negative) and assigns intensity scores (0.0 to 1.0).
- **Example-Driven Analysis**: Guides the sentiment extraction process using predefined examples.
- **File Export**: Saves the extraction results into a structured JSONL file.
- **Visualization**: Generates an HTML visualization of the extraction results for better interpretability.

## Prerequisites

- Python 3.x
- Jupyter Notebook or Google Colab
- `LangExtract` library

## Installation

Install the `LangExtract` library by running the following command in the notebook:

```bash
!pip install langextract
```

## Notebook Steps

1. **Setup**:
   - Install the required `LangExtract` library.
   - Import necessary packages.

2. **Defining the Extraction Rules**:
   - Create a prompt for extracting sentiment phrases.
   - Define attributes for each sentiment, including category and intensity.

3. **Providing Examples**:
   - Supply high-quality examples to guide the model in understanding the extraction rules.

4. **Analyzing the Text**:
   - Provide input text for sentiment analysis.
   - Use the `LangExtract` library to extract sentiment phrases and their attributes.

5. **Saving the Results**:
   - Save the extracted data into a JSONL file.

6. **Visualization**:
   - Generate an HTML file to visualize the extraction results.

## Example Input and Output

### Input Text
```
The city air was thick with the smell of rain and exhaust as Kaelen clutched the faded photograph. A wave of profound sadness washed over him as he remembered happier times. He had to find her. Across the street, a shadowy figure watched from an alley, a flicker of cold amusement in their eyes before they melted back into the darkness.
```

### Extracted Sentiments
- **Phrase**: "profound sadness"
  - **Category**: Negative
  - **Intensity**: 0.9
- **Phrase**: "happier times"
  - **Category**: Positive
  - **Intensity**: 0.7
- **Phrase**: "cold amusement"
  - **Category**: Negative
  - **Intensity**: 0.7

## File Outputs

- **JSONL File**: The extraction results are saved in `extraction_results.jsonl`.
- **HTML File**: The visualization is saved as `visualization.html`.
