# LLM_CNN_Spring2025
Among the evaluated summarization models and decoding techniques.

SWE 422 – Introduction to Large Language Models
Spring 2025 – Homework Report
Students:
Şeyma Altıparmak | B201202051
Emine Nisa Türk | B201202014

## 1. Setup and Methodology
BART and Pegasus. We used a small (1%) portion of the CNN/DailyMail dataset to ensure quicker results while maintaining content diversity.
Experiments were conducted using three decoding strategies:
Greedy Decoding
Beam Search
Sampling (Top-k & Nucleus)
Performance was evaluated with the ROUGE metric.

## 2. Model Comparison
BART (facebook/bart-large-cnn):
Produced fluent summaries, but sometimes repeated phrases.
Beam search was the best decoding option for this model.
Pegasus (google/pegasus-cnn_dailymail):
Generated short, natural, and human-like summaries.
Even greedy decoding gave impressive results thanks to its pretraining.

## 3. ROUGE Evaluation Summary
Pegasus (Greedy) --> Best Overall
BART (Beam Search)	Very Good
BART (Greedy)	Moderate
BART (Sampling)	Unstable / Lower

## 4. Key Observations
Pegasus outperformed BART in both accuracy and natural language quality. Beam search gave the most reliable results overall. Sampling was creative but often inconsistent and off-topic.

## 5. Conclusion
For high-quality and dependable summarization, Pegasus with greedy or beam decoding is the best choice. BART with beam search is a solid alternative. Sampling methods, while diverse, are not reliable for tasks requiring precision.

