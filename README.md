# Leveraging LlamaIndex for Synthetic Financial Data Analysis

This repository contains code for generating synthetic questions based on the content of financial reports, specifically 10-K filings. By utilizing the LlamaIndex library and OpenAI's language model, this project aims to automate the process of extracting meaningful insights from financial documents without the need for manual analysis.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Importance for Financial Analysts](#importance-for-financial-analysts)

## Overview

Generating synthetic data can be a game-changer in financial analysis, enabling analysts to create valuable insights quickly and efficiently. This project focuses on:

- Extracting data from a 10-K financial report.
- Dividing the document into manageable chunks.
- Using a Large Language Model (LLM) to generate diverse and relevant questions.

## Installation

To run this project, you will need to install the necessary packages. You can do this using pip:

```bash
pip install llama-index openai tqdm
```

Make sure you have a valid OpenAI API key and set it in your environment.

## Usage

1. **Download the Financial Report**: The code automatically downloads a 10-K financial report (e.g., Amazon's report).
2. **PDF Chunking**: The report is processed and chunked into smaller sections for analysis.
3. **Question Generation**: The LLM generates synthetic questions based on the text from the report.
4. **Output**: The generated questions are stored in a dictionary with references to their relevant context in the document.

To run the code, simply execute the script in a Python environment that supports Jupyter notebooks or Google Colab.

## How It Works

The code consists of several key steps:

1. **PDF Data Extraction**: The script downloads the specified 10-K financial report and extracts its text content using the LlamaIndex library.

2. **Data Chunking**: The extracted content is processed into smaller sections (nodes) to facilitate question generation.

3. **Synthetic Question Generation**: Using OpenAI's GPT model, the script generates a defined number of questions for each node. These questions encompass key financial concepts, metrics, and specific numerical data from the report.

4. **Output Storage**: The generated questions are stored in a dictionary, with each question linked to its corresponding context.

## Importance for Financial Analysts

Generating synthetic questions can be a game-changer for financial analysts in the following ways:

- **Efficiency**: Saves time in document review and analysis, allowing analysts to focus on interpreting results rather than extracting data.

- **Scalability**: This approach enables the creation of large sets of questions across multiple reports, facilitating comprehensive analyses across different financial documents.

- **Insight Generation**: By asking diverse questions about the report's content, analysts can uncover insights and trends that might not be immediately apparent from the raw data.


