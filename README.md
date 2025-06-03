# Fine-tuning Llama 3 8B for Dialogue Summarization

This project demonstrates how to fine-tune the Llama 3 8B model using Unsloth and LoRA for the task of dialogue summarization. The fine-tuning is performed on the DialogSum dataset.

## Project Description

The goal of this project is to fine-tune a large language model to effectively summarize conversations. We leverage Unsloth for efficient memory management and faster training, and LoRA (Low-Rank Adaptation) for parameter-efficient fine-tuning.

## Dataset

The project uses the [DialogSum dataset](https://huggingface.co/datasets/neil-code/dialogsum-test), a collection of everyday conversations with corresponding summaries.

## Model

*   **Base Model:** `unsloth/llama-3-8b-bnb-4bit`
*   **Fine-tuning Method:** LoRA

## Evaluation

The fine-tuned model is evaluated using the ROUGE metric, comparing the generated summaries to the human-written summaries in the test set.

The evaluation results show a significant improvement in ROUGE scores for the PEFT model compared to the original model:

### rouge1: 10.99% rouge2: 6.85% rougeL: 8.54% rougeLsum: 10.03%
