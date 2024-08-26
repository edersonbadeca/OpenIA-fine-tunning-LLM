# Fine-Tuning GPT-3.5 Turbo with Fictional Patient Histories

![Medical Image](medic.png)

This repository contains the code used to fine-tune the GPT-3.5 Turbo model from OpenAI using fictional patient history data. The goal of this project is to adapt a language model to provide more accurate responses in a medical context while maintaining data privacy, as all data used is fictional.

## Overview

The main script, `fine_tune.py`, handles the entire fine-tuning process, from data preprocessing to model training. The code also includes cost estimation for training and data validation before being sent for fine-tuning.

### Script Features

- **Data Splitting**: Creates train, validation, and test splits from the dataset.
- **Token Counting**: Calculates the number of tokens in each medical report to estimate the fine-tuning cost.
- **Data Validation**: Checks if the prompts are within token limits and contain all necessary fields.
- **Data Formatting**: Converts the data into a format suitable for training, according to OpenAI guidelines.
- **Training**: Performs fine-tuning of the GPT-3.5 Turbo model using the prepared data.

## Repository Structure

- `fine_tune.py`: Main script that handles the fine-tuning process.
- `data/`: Directory where the fictional data is stored.
- `models/`: Directory where the fine-tuned models are saved.
- `train_data.jsonl` and `val_data.jsonl`: Formatted data files for training and validation.

## How to Use

### Prerequisites

- Python 3.8 or higher
- Libraries listed in `requirements.txt`
- OpenAI account with API access for fine-tuning

### Execution Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/edersonbadeca/OpenIA-fine-tunning-LLM.git
   

