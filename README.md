# AI Text Summarizer

## Overview

AI Text Summarizer is a web application built using Python, Streamlit, and Hugging Face Transformers. It summarizes long articles and paragraphs into shorter, meaningful text using a pre-trained DistilBART model.

## Features

- Summarizes long articles and paragraphs.
- Uses a pre-trained Hugging Face summarization model.
- Allows users to configure minimum and maximum summary lengths.
- Displays the original and summarized word counts.
- Calculates text reduction percentage.
- Provides an option to download the generated summary as a text file.
- Includes a simple and interactive web interface.

## Technologies Used

- Python
- Streamlit
- Hugging Face Transformers
- PyTorch
- DistilBART CNN model

## Project Structure

```text
summarizer/
├── app.py
├── requirements.txt
└── README.md
```

## Installation

### 1. Clone the Repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the Project Folder

```bash
cd summarizer
```

### 3. Install the Required Libraries

```bash
python -m pip install -r requirements.txt
```

## Run the Application

Start the Streamlit application using the following command:

```bash
python -m streamlit run app.py
```

The application will open in your default browser. If it does not open automatically, visit:

`http://localhost:8501`

## How It Works

1. The user enters an article or paragraph into the text area.
2. The application loads the pre-trained DistilBART model through the Hugging Face Transformers Pipeline.
3. The model generates a summary based on the input text and selected length settings.
4. The application displays the generated summary.
5. The user can view word counts, text reduction percentage, and download the summary.

## Model Information

- Model: `sshleifer/distilbart-cnn-12-6`
- Task: Text Summarization
- Framework: Hugging Face Transformers Pipeline
- Execution: PyTorch

The model is downloaded automatically from Hugging Face when it is loaded for the first time. An internet connection is required for the initial download.

## Requirements

The project dependencies are listed in `requirements.txt`:

```text
streamlit
transformers<5
torch
```

## Future Improvements

- Support for PDF and document uploads.
- Multiple language summarization.
- Summary history.
- Improved user interface.
- Adjustable summary compression levels.
