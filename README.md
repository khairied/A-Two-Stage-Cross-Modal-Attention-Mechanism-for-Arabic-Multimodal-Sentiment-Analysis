# 🚨 The first Arabic multimodal sentiment analisys dataset  
### A-Two-Stage-Cross-Modal-Attention-Mechanism-for-Arabic-Multimodal-Sentiment-Analysis🧠🖼️📝
## Note that the full code will be availabrl after paper publication
## 📌 Overview
This repository provides a curated dataset and an experimental notebook for **Arabic multimodal sentiment classification**.  
The dataset includes **tweet IDs**, **labels (Negative/Positive/Neutral)**, and **source dataset names**, enabling researchers and students to explore **image–text sentiment analysis** on Arabic social media platforms.

The accompanying notebook demonstrates how to load the dataset, conduct ablation experiments, and evaluate multimodal learning architectures in a reproducible manner.

---

## 📂 Dataset Format
The dataset is released as "MafiaNetDataset.csv" with the following structure:

- `id` – Twitter Tweet ID  
- `label` – Class label (`0` = Fake, `1` = Real)  
- `dataset` – Source dataset name  

✔️ Only Tweet IDs are shared to fully comply with Twitter/X data-sharing policies.

---

## 🗂️ Data Collection
- Arabic tweets were collected from **multiple misinformation-related sources**, including COVID-19 content, rumors, and fake news datasets.
- Data acquisition was performed using the **Twitter API** (e.g., Tweepy) or web scraping tools.
- Labels were inherited from **existing Arabic unimodal annotated datasets**, enabling scalable multimodal annotation with minimal manual effort.
- Text and media content can be programmatically retrieved using the provided tweet IDs.

## 📈 Dataset Content Statistics

| Class     | # of Tweets | Total Words | # Unique Words | Avg Words |
|------------|--------------|--------------|----------------|------------|
| Positive   | 551          | 8432         | 4405           | 15.30      |
| Negative   | 671          | 10887        | 5238           | 16.23      |
| Neutral    | 500          | 4994         | 2843           | 9.99       |
| **Total**  | **1722**     | **24313**    | **10527**      | **14.12**  |
## 📊 Dataset Statistics

| Dataset   | # Positive | # Negative | # Neutral | Total |
|------------|------------|------------|------------|--------|
| Gold       | 39         | 42         | 74         | 155    |
| Arcust     | 27         | 154        | 0          | 181    |
| Patience   | 154        | 186        | 0          | 340    |
| Sarcasm    | 178        | 153        | 299        | 630    |
| Topics     | 153        | 136        | 127        | 416    |
| **Total**  | **551**    | **671**    | **500**    | **1722** |


---

## 🧪 Notebook (Ablation Study)
The provided notebook includes the following experimental settings:
- 📌 **Data Collection** Hydrate_TweetIDs.ipynb
- 📝 **Text Encoder Only** CNN Image Encoder Only.ipynb and Vision Encoder Only.ipynb   Hydrate_TweetIDs.ipynb
- 🖼️ **Image Encoder Only** Image Encoder only.ipynb
- ❌ **MAFIA-Net without MARBERTv2** Without Marbert.ipynb
- ❌ **MAFIA-Net without EfficientNet-B1** Without efficientnetb1.ipynb
- ❌ **MAFIA-Net without HCMA** Without HCMA.ipynb
- ❌ **MAFIA-Net without VGTA** Without VGTA.ipynb
- ✅ **Full MAFIA-Net Model** MafiaNet.ipynb

These experiments highlight the contribution of each module to multimodal fake news detection.

---

## 🔐 Accessing the Full Dataset
Due to Twitter/X content redistribution policies, the **full hydrated dataset** is not publicly released.

📩 To request access, please fill out the following Google Form:  
👉 https://docs.google.com/forms/d/1RAmKljzO_0poMIDWBeHqbJchwi_RfAyMvlasbwY46E4/edit

Requests are intended for **research and academic use only**.

---

## 📚 Citation
If you use this dataset or code in your research, please cite:

@article{mafianet2026,
  title={MAFIA-Net: Multimodal Arabic Fake-news Identification via Hybrid Attention Networks},
  author={},
  journal={},
  year={2026}
}

---

## ⚖️ License
This repository is released for **research and educational purposes**.  
Tweet IDs are shared in accordance with Twitter/X Developer Policy.

