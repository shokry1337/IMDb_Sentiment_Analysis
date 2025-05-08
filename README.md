# IMDB Sentiment Analysis
## LLaMA 3.1 8B x GPT-4o-Mini

This project explores the use of large language models for sentiment classification of movie reviews. By leveraging both the `LLaMA-3.1-8B` and the `GPT-4o-Mini` models via the `g4f` interface and comparing their performance.

This notebook demonstrates an alternative to traditional supervised machine learning techniques by prompting generative models to act as zero-shot sentiment analyzers with no need of extra training, or fine-tuning.

---

### Dataset

This project uses the [Large Movie Review Dataset v1.0 (aclImdb)](https://ai.stanford.edu/~amaas/data/sentiment/), which contains 50,000 movie reviews labeled as either positive or negative.

---

### Results

The following table shows the result of comparing both models using 4 different metrics, `Accuracy`, `Precision`, `Recall`, and `F1-Score` after processing 1000 reviews each. This demonstrates that the difference between the two models' ability to perform contextual understanding is minimal.

|              | Accuracy | Precision | Recall | F1-Score |
|--------------|----------|-----------|--------|----------|
| Llama-3.1-8B | 0.9314   | 0.9801    | 0.8931 | 0.9346   |
| GPT-4o-Mini  | 0.9364   | 0.9722    | 0.9072 | 0.9386   |