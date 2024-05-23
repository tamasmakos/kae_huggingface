# Bias Detection in Scientific Abstracts

This project involves downloading abstracts of papers published in 2023 and using the Huggingface API to detect biases in the text. Additionally, it analyzes whether certain text statistics correlate with the detected biases using a large language model (LLM). The project also includes topic modeling to investigate if certain categories have a higher bias rate.

## Overview

The project performs the following tasks:
- Downloads abstracts of papers published in 2023.
- Detects biases in the text using Huggingface API models.
- Computes various text statistics to analyze readability and complexity.
- Correlates text statistics with detected biases.
- Uses topic modeling to categorize the abstracts and identify bias trends.

## Features

### Text Statistics
The following text statistics are computed for each abstract:
- **Flesch Reading Ease**
- **Flesch-Kincaid Grade**
- **SMOG Index**
- **Coleman-Liau Index**
- **Automated Readability Index**
- **Dale-Chall Readability Score**
- **Difficult Words**
- **Linsear Write Formula**
- **Gunning Fog Index**
- **Text Standard**
- **Fernandez Huerta**
- **Szigriszt Pazos**
- **Gutierrez Polini**
- **Crawford**
- **Gulpease Index**
- **Osman**

### Bias Detection APIs
The following Huggingface models are used for bias detection:
- `valurank/distilroberta-bias`
- `amedvedev/rubert-tiny2-cognitive-bias`

### Topic Modeling API
The Huggingface model used for topic classification:
- `valurank/distilroberta-topic-classification`
