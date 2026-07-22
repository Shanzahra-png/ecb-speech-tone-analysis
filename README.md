## Model Architecture

![FinBERTGate Fusion Architecture](figures/finbert_gate_fusion_architecture.png)
# ECB Speech Tone Analysis using FinBERT

## Quantifying ECB Speech Tone and Its Influence on the European Bond Market Through Financial Signal Extraction

This repository contains the implementation of my MPhil Data Science thesis. The project investigates how the tone of European Central Bank (ECB) speeches influences the German 10-Year Government Bond Yield using transformer-based Natural Language Processing (NLP) and Deep Learning techniques.

---

## Project Overview

Central bank communication plays a significant role in financial markets. This research develops an automated framework to classify the monetary policy tone of ECB speeches and analyze their relationship with bond market movements.

The project combines Financial NLP, Deep Learning, and Financial Time Series Analysis to extract meaningful signals from central bank speeches.

---

## Research Objectives

- Quantify the tone of ECB speeches using FinBERT.
- Analyze the impact of ECB communication on German 10-Year Government Bond Yields.
- Build an end-to-end Financial NLP pipeline.
- Evaluate the relationship between speech tone and market reaction.

---

## Methodology

The workflow of this project is:

1. Collect ECB speeches.
2. Fetch Germany 10-Year Bond Yield data.
3. Preprocess financial text.
4. Extract contextual embeddings using FinBERT.
5. Generate speech-level sentiment scores.
6. Align speeches with bond yield movements.
7. Train and evaluate the classification model.
8. Analyze the relationship between predicted tone and market response.

---

### Architecture Overview

The proposed FinBERTGate Fusion architecture combines three complementary information sources:

- **FinBERT Branch:** Extracts contextual semantic representations from ECB speeches.
- **Loughran–McDonald Branch:** Captures domain-specific financial sentiment using dictionary-based features.
- **Temporal Branch:** Incorporates German 10-Year bond market context, including yield level, daily change, and volatility.

The extracted features are fused using a learnable gating mechanism before being passed to a classifier that predicts three monetary policy tone classes:

- 🟦 Dovish
- ⚪ Neutral
- 🟥 Hawkish

---
## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- FinBERT
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## Repository Structure

```
ecb-speech-tone-analysis/
│
├── ECB_Speech_Tone_Analysis.ipynb
├── README.md
├── requirements.txt
├── figures/
├── docs/
└── results/
```

---

## Dataset

This project utilizes:

- European Central Bank (ECB) Speeches
- Germany 10-Year Government Bond Yield
- Publicly available financial data sources

---

## Research Areas

- Natural Language Processing
- Financial NLP
- Deep Learning
- Machine Learning
- Financial Signal Extraction
- Transformer Models

---

## Future Work

Future improvements include:

- Large Language Models (LLMs)
- Cross-lingual Financial NLP
- Real-time Central Bank Speech Analysis
- Explainable AI (XAI)
- Multi-modal Financial Intelligence

---

## Author

**Shan Zahra**

MPhil Data Science  
Bahauddin Zakariya University, Pakistan

Research Interests:

- Artificial Intelligence
- Natural Language Processing
- Financial AI
- Deep Learning
- Machine Learning

---

## Citation

If you find this repository useful for academic research, please consider citing the associated thesis.

---

## License

This project is released for research and educational purposes.
