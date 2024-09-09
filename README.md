# Text Classification with Fine-Tuning LLMs

## Overview

This repository focuses on text classification using various fine-tuning techniques for Large Language Models (LLMs). It explores the use of LoRA (Low-Rank Adaptation) and other Parameter-Efficient Fine-Tuning (PEFT) methods, with models such as BERT and RoBERTa. Additionally, the project includes deployment of these models using Streamlit and Gradio.

## Directory Structure

Here is an overview of the directory structure used in this project:
```
LLM-PEFT-Text-Classification-Repo 
│
├── data/
│     ├── raw/ # Raw data files 
│     ├── processed/ # Processed data files 
│     └── preprocessing/ # Scripts for data preprocessing and augmentation 
│
├── models/ 
│     ├── base/ # Base models (e.g., BERT, RoBERTa) 
│     ├── lora/ # LoRA-specific scripts and configurations 
│     └── peft/ # Other PEFT techniques scripts and configurations 
│
├── notebooks/ # Jupyter notebooks for experimentation and analysis 
│     ├── scripts/ 
│     ├── train.py # Script to train models 
│     ├── evaluate.py # Script to evaluate models 
│     ├── infer.py # Script for inference 
│     ├── utils.py # Utility functions and helpers 
│     └── config.yaml # Configuration file for model parameters and training settings 
│
├── deployment/ 
│     ├── streamlit/ # Streamlit deployment scripts and configurations 
│     └── gradio/ # Gradio deployment scripts and configurations 
│
├── tests/ # Unit tests and validation scripts 
│     ├── test_train.py # Tests for training functionality 
│     ├── test_evaluate.py # Tests for evaluation functionality 
│     └── test_infer.py # Tests for inference functionality 
│
├── logs/ # Logs and experiment tracking 
│
├── requirements.txt # Python dependencies   
├── Dockerfile # Dockerfile for containerization 
├── README.md # Project overview and instructions 
└── .gitignore # Git ignore file
```


## Getting Started

To get started with this project:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/arshraj-r/LLM-PEFT-Text-Classification-Repo.git
   cd LLM-PEFT-Text-Classification-Repo
2. **Install Dependencies:**:
   ```bash
   pip install -r requirements.txt
3. **Configure the Environment:**: Update the config.yaml file with the desired model parameters and training settings.
4. **Training Models:** : Run the training script:
   ```bash
   python scripts/train.py --model_name <model_name> --num_train_epochs <epochs> --batch_size <batch_size> --warmup_steps <steps>
5. **Evaluating Models:** : Run the evaluation script:
   ```bash
   python scripts/evaluate.py --model_name <model_name>
6. **Performing Inference:**:  Run the inference script:
   ```bash
   python scripts/infer.py --model_name <model_name>
7. **Deploying Models:** : Follow the instructions in the deployment/ directory for deploying the models using Streamlit or Gradio.


