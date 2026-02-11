# LLM Preference Modeling (Chatbot Arena)

This project builds a reproducible baseline for predicting **human preference between two LLM responses** using the Chatbot Arena dataset.

## Objective
Given a prompt and two candidate responses, predict which response a human judge would prefer:
- Response A wins
- Response B wins
- Tie

Evaluation metric: **Multiclass Log Loss**

## Approach
- Constructed TF-IDF text representations for prompt–response pairs
- Implemented multinomial logistic regression baseline
- Developed **pairwise preference modeling (A − B)** to capture relative response quality
- Performed bias analysis revealing **verbosity-driven preference tendencies**
- Introduced a **length-difference feature** to mitigate verbosity bias
- Conducted ablation experiments demonstrating consistent performance improvements

## Results
Pairwise modeling and bias-aware feature engineering improved validation log-loss compared to the concatenation baseline.

## Future Work
- Transformer embedding-based preference scoring
- Reward-model fine-tuning
- Bias-corrected preference optimization

## Repository Structure
