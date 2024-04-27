**Emotion Classification with Parameter-Efficient Fine-Tuning**

This project demonstrates the use of parameter-efficient fine-tuning (PEFT) to adapt a GPT-2 language model for the task of emotion classification. The  Hugging Face PEFT library is used to fine-tune the model, resulting in improved performance without requiring extensive computational resources.

**Project Overview**

Lightweight fine-tuning is a valuable technique for customizing large language models. In this project, I've applied PEFT to fine-tune a pre-trained GPT-2 model for emotion classification, following these key steps:

- Loaded a pre-trained GPT-2 model and evaluated its baseline performance on the emotions dataset.
- Performed parameter-efficient fine-tuning using the LoRA technique.
- Evaluated the fine-tuned model using the Trainer.evaluate method, demonstrating improved performance compared to the original model.

**Dataset**

Hugging Face Emotions Dataset: Used for training and evaluation (https://huggingface.co/datasets/emotion). This dataset features text samples labeled with six core emotions: sadness, joy, love, anger, fear, and surprise.

**Model**

GPT-2: A pre-trained Transformer-based language model from Hugging Face.

**Fine-Tuning Technique**

LoRA (Low-Rank Adaptation): A parameter-efficient fine-tuning technique that introduces trainable, low-rank decomposition matrices into the model to adjust existing weights.

**Results**

Parameter-efficient fine-tuning using LoRA led to the following improvements in the GPT-2 model's performance on the emotion classification task:

- Accuracy increased by 85.2%
- Loss reduced by 96.8%
- F1 score improved by 91.95%
