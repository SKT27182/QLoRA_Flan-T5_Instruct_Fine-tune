# QLoRA Fine Tuning of Large Languge Model on Open-Orca dataset

## Introduction

- In this project I have fine-tuned a Flan-T5 model on Open-Orca dataset. The model is trained on a single GPU with 16GB memory. The model is trained for 6 epochs with a batch size of 16. 

- I have used QLoRA technique to quantize the model. The model is quantized to 4-bit precision. For the linear layers, I have used nf4 quantization scheme. While computation used the bfloat16 format.

- I have also trained the head of the Flan-T5 along with LoRA layers. Used pytorch for training and BitsAndBytes for quantization.


## Dataset

- The dataset is available at [Open-Orca](https://huggingface.co/datasets/Open-Orca/OpenOrca) and the Preprocessed dataset is available at [SKT27182/Preprocessed_OpenOrca](https://huggingface.co/datasets/SKT27182/Preprocessed_OpenOrca).
