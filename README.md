# Fine-tuning Vicuna-7b for Text Summarisation

## Project Overview
This project focuses on fine-tuning the Vicuna-7b large language model for text summarisation tasks, utilising Parameter-Efficient Fine-Tuning (PEFT) methods. Techniques such as 4-bit quantisation and Low Rank Adaptation (LoRA) are employed to optimise computational efficiency. This implementation leverages Hugging Face's Transformers, BitsAndBytes, and Accelerate libraries, and is executed on a Kaggle notebook environment.

### Features
- Utilisation of the Vicuna-7b language model from Hugging Face's model hub.
- Implementation of 4-bit quantisation and LoRA for enhanced training efficiency.
- Application of Supervised Fine Tuning (SFT) and a sequence length cap of 1024 tokens for improved performance.
- Adjustment of data types in normalisation layers for better numerical stability.

## Installation

Ensure you have Python 3.x installed on your system. You can then install the required libraries using the following commands:

```bash
pip install transformers
pip install -q -U bitsandbytes
pip install -q -U git+https://github.com/huggingface/transformers.git
pip install -q -U git+https://github.com/huggingface/peft.git
pip install -q -U git+https://github.com/huggingface/accelerate.git

