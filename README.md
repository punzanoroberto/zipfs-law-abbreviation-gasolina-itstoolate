# zipfs-law-abbreviation-gasolina-itstoolate
# Overview

This project investigates whether Zipf's Law of Abbreviation holds for specific text genres in English and Spanish. It compares the degree to which both languages conform to the law by analyzing the statistical relationship between word frequency and word length. This project was developed by Roberto Punzano as a solo project, with GenAI used as a supporting tool.

# Key Insights

The study confirmed a negative correlation between word frequency and length in both datasets, with the Spanish corpus showing a stronger adherence to Zipf’s Law of Abbreviation than the English corpus.

# Dataset

The experiments use lyrics from two distinct musical works to represent different languages:
* **English**: "It's Too Late" by Carole King.
* **Spanish**: "Gasolina" by Daddy Yankee.
* Data was processed from raw text files and filtered to include only alphabetic tokens.

# Methods

The analysis was implemented in Python using the following methodology:
* **Tokenization**: Performed using `spaCy` with language-specific models (`en_core_web_sm` and `es_core_news_sm`).
* **Frequency Mapping**: A dictionary was created for each language, mapping every unique word to its number of occurrences and its character length.
* **Statistical Analysis**: Spearman Rank Correlation Coefficient was calculated using `SciPy` to measure the strength and direction of the relationship between frequency and length.

# Results

Zipf's Law of Abbreviation was validated for both languages:
* **English Results**: Spearman rho ($\rho$) of -0.356 with a p-value of 0.0011.
* **Spanish Results**: Spearman rho ($\rho$) of -0.506 with a p-value of 6.76e-09.
* The Spanish data showed a more pronounced negative correlation, suggesting a stricter optimization of word length relative to frequency in this specific text.

# Reproducibility

The code is provided in a Jupyter Notebook format, including all steps from data ingestion to statistical output. Dependencies include `spacy`, `scipy`, and the relevant spaCy language models.

# Limitations

The analysis is limited by the relatively small sample size of the song lyrics. Future research could include larger corpora or different genres to determine if these correlation strengths generalize across entire languages or remain specific to the selected musical texts.
