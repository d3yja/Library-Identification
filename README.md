# Historical Library Metadata Extraction and Genre Classification

This project focuses on the extraction, structuring, and classification of metadata from historical European library catalogs. We combine OCR, large language models (LLMs), and transformer-based classifiers (specifically BERT) to digitize, clean, and analyze data from early printed book inventories. This project was done under the mentorship of Mehta+ and Prof Colin Wildler (University of South Carolina). The project can also be found on this repository: https://github.com/MehtaPlusTutoring/studentprojects/tree/main/aimlresearchbootcamp/2025

## 🧠 Project Goals

- Extract metadata from scanned historical library records using OCR and LLMs.
- Structure the extracted data into a machine-readable format (JSON).
- Train a transformer-based classifier to predict book genres using fields like:
  - `BookName`
  - `Library Name`
  - `Description`
- Evaluate model performance and address class imbalance issues.

## 🔍 Motivation

Historical library catalogs from monasteries, universities, and bureaucratic institutions are key to understanding European intellectual history. Digitizing and classifying their contents enables scalable access for historians, linguists, and digital humanities researchers.

## 🛠️ Tools and Technologies

- Python (pandas, scikit-learn, transformers)
- BERT (fine-tuned for genre classification)
- OCR (Tesseract or ABBYY FineReader)
- OpenAI LLMs for metadata parsing and cleaning
- Jupyter Notebooks for prototyping
- LaTeX (Overleaf) for paper/poster formatting


## 📊 Evaluation Metrics

We use macro-averaged metrics due to class imbalance:

- **Precision**: `TP / (TP + FP)`
- **Recall**: `TP / (TP + FN)`
- **F1-Score**: Harmonic mean of precision and recall

> Achieved strong performance on high-support genres; performance was limited for rare classes due to class imbalance and minimal context.

## 🚧 Challenges

- Dealing with OCR errors in older, degraded texts.
- Ambiguity and inconsistency in historical naming conventions.
- Handling class imbalance across genre categories.
- No labeled training data.

## ✅ Current Status

- ✅ OCR pipeline implemented and tested
- ✅ LLM-based metadata extraction working with historical PDFs
- ✅ BERT classifier trained and evaluated

## 🤝 Acknowledgements

We are grateful to Professor Colin Wilder for supplying the original data and helping us define our task
framework, and Haripriya and Bhagirath Mehta from MehtA+ Tutoring for guiding us through this process.

## 📜 Citation


[Ma et al.(2024)] Zhiwei Ma, Javier E. Santos, Greg Lackey, Hari Viswanathan, and Daniel O’Malley.
“Information Extraction from Historical Well Records Using a Large Language Model.” Scientific Reports,
vol. 14, article 81846, 2024. https://doi.org/10.1038/s41598-024-81846-5
[Vaswani et al.(2017)] Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan
N. Gomez, Lukasz Kaiser, and Illia Polosukhin. “Attention Is All You Need.” In Advances in Neural
Information Processing Systems, vol. 30, 2017. https://arxiv.org/abs/1706.03762


