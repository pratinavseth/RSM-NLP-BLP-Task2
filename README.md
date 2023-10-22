<div align="center">
  
# RSM-NLP at BLP-2023 Task 2: Bangla Sentiment Analysis using Weighted and Majority Voted Fine-Tuned Transformers

Accepted at the 1st Workshop on Bangla Language Processing, EMNLP 2023

</div>

# Sentiment Analysis of Bangla Social Media Posts
This repository contains our codes for Shared Task 2 at the EMNLP 2023 BLP Workshop - Sentiment Analysis of Bangla Social Media Posts. The goal of the task is to promote work in Bangla Sentiment Analysis and identifying the polarity of social media content by determining whether the sentiment expressed in the text is positive, negative or neutral.
## Overview
Our approach involved experimenting with and finetuning various pre-trained BERT-based models on our downstream task, followed by using ensembling techniques to create a model that outperforms individual baseline model scores. 
### Pretrained models
The pretrained models used for the downstream task of Sentiment Classification involve:
- [DistilBERT (multilingual-cased)](https://huggingface.co/distilbert-base-multilingual-cased)
- [RoBERTa](https://huggingface.co/roberta-base)
- [sagorsarker/BanglaBERT](https://huggingface.co/sagorsarker/bangla-bert-base)
- [Indic-abusive-AllInOne-MuRIL](https://huggingface.co/Hate-speech-CNERG/indic-abusive-allInOne-MuRIL)
- [Bengali-abusive-MuRIL](https://huggingface.co/Hate-speech-CNERG/bengali-abusive-MuRIL)
- [BanglaBERT](https://huggingface.co/csebuetnlp/banglabert_small)
- [BanglishBERT](https://huggingface.co/csebuetnlp/banglishbert)

### Ensembling techniques
Ensembling techniques were applied to the top 3, top 5 and all the pretrained models to improve the performance of the predictive models. Two ensembling techniques were applied:
- Majority-voting
- Weighted ensemble
