# Finetuning-LLM-for-Medical-conversation
This project focuses on fine-tuning Large Language Model (Llama-2-7B) for medical conversations. It involves preprocessing raw medical conversation data, training language models using PyTorch and Hugging Face Transformers, and fine-tuning pre-trained models on medical conversation datasets for domain-specific tasks.
# Features
## Data Preprocessing: 
Transforming raw medical conversation data.
## Model Training: 
Training language models.
## Fine-tuning: 
Fine-tuning the pre-trained LLAMA-2-7B model on medical conversation datasets.
# Installations
Install the required dependencies from the requirements.txt file:

pip install -r requirements.txt
# Usage
## Data Preprocessing: 
Transform raw medical conversation data into a model-readable format.
## Model Training: 
Train language models using PyTorch and Hugging Face Transformers.
## Fine-tuning: 
Fine-tune the pre-trained LLAMA-2-7B model on medical conversation datasets for domain-specific tasks.
# Tuning Parameters
 Tuning Parameters:
Following tuning parameters are used in our model

QLORA: ‘Lora-r =64’, ‘Lora-a = 16’ and Lora-dropout is used.

Bits and Bytes: 4 bit quantization is used for loading weights in compressed formats.

Training Arguments: Batch size per GPU at training=4, Gradient-accumulation steps=1, Learning rate = 2e-4, max-gradient norm= 0.3

Trainer Configuration: For supervised fine-tuning, SFT Trainer is configured. Default maximum
sequence length is used. 
