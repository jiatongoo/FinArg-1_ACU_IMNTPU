# FinArg-1: Argument Unit Classification Task

## Introduction
In recent years, argument mining has drawn significant attention, particularly in the financial domain, where analyzing text deeply can reveal hidden sentiments and intentions. The FinArg-1 task, introduced in the NTCIR-17 competition, focuses on classifying argument units in financial documents into either premises or claims. This helps us better understand the argumentative structures in financial reports and presentations.

For this task, we fine-tuned three models: RoBERTa, BERT, and GPT-3.5 Turbo. These models helped us accurately classify argument units and provided strong support for understanding the complexity of market sentiment and financial arguments.

## Dataset Information
- **Train:** 7753 sentences
- **Dev:** 969 sentences
- **Test:** 968 sentences

Each data entry consists of two fields: `sentence` and `prediction`. The prediction has two classes:
- **Class 0:** Premise
- **Class 1:** Claim

## Contribution
1. **Fine-tuning Argument Unit Classification Models:**  
   We fine-tuned three models—RoBERTa, BERT, and GPT-3.5 Turbo—for classifying argument units. Our RoBERTa model performed best, achieving a Micro-F1 score of 76.06%, Macro-F1 score of 76.05%, and Weight-F1 score of 76.07%, showing excellent precision and stability in sentiment classification. The BERT model closely followed with a Micro-F1 of 75.44%, Macro-F1 of 75.31%, and Weight-F1 of 75.40%. Although GPT-3.5 Turbo performed weaker in this task (Micro-F1 of 56.97%), it provided a valuable benchmark as a generative model, offering important comparative insights for future research.

2. **Deep Analysis of Financial Text Sentiment:**  
   Our models successfully assigned single sentiment labels to financial texts, helping to reveal how market sentiment spreads through public discussions. This analysis provides investors and financial analysts with more accurate decision-making tools and highlights the potential of deep learning models in financial argument mining and sentiment analysis.

3. **Performance in NTCIR-17 Competition:**  
   Our RoBERTa model ranked 8th in the NTCIR-17 competition, demonstrating its effectiveness in financial sentiment analysis. The BERT model also performed well, closely matching RoBERTa's results, providing strong support for future research. Despite GPT-3.5 Turbo's relatively weaker performance, its potential as a generative model remains significant, offering valuable references for future applications in financial texts.
