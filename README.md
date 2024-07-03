## resource
https://www.kaggle.com/competitions/lmsys-chatbot-arena

## Objective:
Predict which responses users will prefer in a head-to-head battle between chatbots powered by LLM.

## Dataset:

Collected from Chatbot Arena.
Users chat with two anonymous LLMs and choose the answer they prefer.

## Challenge Context:

Aligns with "reward models" or "preference models" in reinforcement learning from human feedback (RLHF).
Addresses biases such as position bias, verbosity bias, and self-enhancement bias.

## Evaluation Metric:

- Submissions are evaluated based on the log loss between the predicted probabilities and the ground truth values.

- The output should be probabilities for each of the three classes: model A winner, model B winner, tie.


## Notebooks Overview
- basic-model.ipynb: A baseline model where features are statistical values based on the length of text responses.
- llama-3-instruct.ipynb: Inference notebook with instruction-tuned LLaMA3.
- transformer_base_model.ipynb: Notebook for training and evaluating different transformer models. Includes fine-tuning BERT-base, Longformer, and DeBERTaV3-base.
- transformer-inference.ipynb: Notebook for inference on the test dataset using already trained models.
