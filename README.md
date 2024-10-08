# Leveraging LlamaIndex for Synthetic Financial Data Analysis

This repository contains code for generating synthetic questions based on the content of financial reports, specifically 10-K filings. By utilizing the LlamaIndex library and OpenAI's language model, this project aims to automate the process of extracting meaningful insights from financial documents without the need for manual analysis.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
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

## Code Explanation

The main components of the code are as follows:

1. **Importing Libraries**: The necessary libraries, including `llama-index`, `OpenAI`, and `tqdm`, are imported.

2. **PDF Data Extraction**: The script downloads the 10-K report and extracts its content into a structured format.

3. **Chunking the Data**: The document is divided into smaller nodes for easier processing.

4. **Generating Questions**: 
   - A prompt template is created to guide the LLM in generating questions.
   - The LLM is called to produce a specified number of questions for each chunk of the document.
   - The generated questions are cleaned and stored alongside their context.

## Importance for Financial Analysts

This tool is designed to assist financial analysts by:

- **Automating Insights**: Quickly generates relevant questions to guide analysis, reducing manual effort.
- **Enhancing Understanding**: Helps identify key metrics and concepts within financial reports, leading to deeper insights.
- **Improving Efficiency**: Saves time in document review and analysis, allowing analysts to focus on interpreting results rather than extracting data.

