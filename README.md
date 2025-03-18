# Taming LLMs with Groq API

## Overview
This project implements a content classification and analysis tool using the Groq API. It applies structured prompt engineering, confidence analysis, and streaming responses to control model completions and extract precise insights from LLM-generated content.

## Learning Objectives
By completing this project, you will:
- Create structured prompts to control model behavior.
- Implement techniques for managing and optimizing model completions.
- Use streaming responses for efficiency.
- Analyze log probabilities to evaluate confidence in model responses.
- Compare different prompt strategies for classification tasks.

## Requirements
### Prerequisites
- Python programming experience
- Basic understanding of HTTP APIs
- Familiarity with prompt engineering concepts
- A Groq API key

### Setup Instructions
1. Create a new Python project directory.
2. Install the required dependencies using pip:
   ```sh
   pip install groq python-dotenv
   ```
3. Create a `.env` file in your project directory and add your Groq API key:
   ```sh
   GROQ_API_KEY=your_api_key_here
   ```
4. Place the Python script (`taming_llm.py`) inside the project directory.

## Features
This project consists of the following functionalities:

### 1. Basic Completion
- Sets up the Groq API client.
- Implements a function to generate completions from input prompts.
- Handles API errors and rate limits.

### 2. Structured Completions
- Creates structured prompt templates.
- Extracts specific sections from completions using start/end markers.
- Implements streaming response handling to stop generation at a specified pattern.

### 3. Classification with Confidence Analysis
- Classifies input text into predefined categories.
- Uses structured prompts to enforce consistent responses.
- Analyzes the model’s confidence using log probability data.
- Filters results based on confidence thresholds.

### 4. Prompt Strategy Comparison
- Implements three prompt strategies for classification:
  - Basic direct-question prompt.
  - Structured format prompt.
  - Few-shot prompt with example classifications.
- Runs the same inputs through all strategies.
- Compares accuracy, confidence, and response characteristics.
- Visualizes the comparison results.

## Usage
1. Run the script:
   ```sh
   python taming_llm.py
   ```
2. Follow the prompts to input text for classification and analysis.
3. View the output, which includes structured classifications and confidence scores.

## Deliverables
- Python script implementing all features.
- A report including:
  - Implementation details and methodology.
  - Screenshots of the tool in action.
  - Analysis of prompt strategy effectiveness.
  - Discussion of encountered challenges and solutions.

## Extra Credit (Optional)
- Implement dynamic confidence threshold calibration.
- Compare results across different Groq models.
- Create a simple web interface using Streamlit or Flask.

## Submission
- Submit your code via a private GitHub repository.
- Ensure your repository includes:
  - A clear README (this file).
  - Well-documented code.
  - A `.env.template` file (do **not** include your actual API key).
- Submit your report as a PDF.

**Due Date:** March 10, 2025, at 23:59.

Good luck!

