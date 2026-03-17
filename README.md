# zipfs-law-abbreviation-gasolina-itstoolate
# Overview

[cite_start]This project investigates whether Zipf's Law of Abbreviation holds for specific text genres in English and Spanish[cite: 2]. [cite_start]It compares the degree to which both languages conform to the law by analyzing the statistical relationship between word frequency and word length[cite: 3]. [cite_start]This project was developed by Roberto Punzano as a solo project, with GenAI used as a supporting tool[cite: 22].

# Key Insights

[cite_start]The study confirmed a negative correlation between word frequency and length in both datasets, with the Spanish corpus showing a stronger adherence to Zipf’s Law of Abbreviation than the English corpus[cite: 22].

# Dataset

The experiments use lyrics from two distinct musical works to represent different languages:
* [cite_start]**English**: "It's Too Late" by Carole King[cite: 22].
* [cite_start]**Spanish**: "Gasolina" by Daddy Yankee[cite: 22].
* [cite_start]Data was processed from raw text files and filtered to include only alphabetic tokens[cite: 22].

# Methods

The analysis was implemented in Python using the following methodology:
* [cite_start]**Tokenization**: Performed using `spaCy` with language-specific models (`en_core_web_sm` and `es_core_news_sm`)[cite: 12, 22].
* [cite_start]**Frequency Mapping**: A dictionary was created for each language, mapping every unique word to its number of occurrences and its character length[cite: 22].
* [cite_start]**Statistical Analysis**: Spearman Rank Correlation Coefficient was calculated using `SciPy` to measure the strength and direction of the relationship between frequency and length[cite: 22].

# Results

[cite_start]Zipf's Law of Abbreviation was validated for both languages[cite: 14, 22]:
* [cite_start]**English Results**: Spearman rho ($\rho$) of -0.356 with a p-value of 0.0011[cite: 22].
* [cite_start]**Spanish Results**: Spearman rho ($\rho$) of -0.506 with a p-value of 6.76e-09[cite: 22].
* [cite_start]The Spanish data showed a more pronounced negative correlation, suggesting a stricter optimization of word length relative to frequency in this specific text[cite: 22].

# Reproducibility

[cite_start]The code is provided in a Jupyter Notebook format, including all steps from data ingestion to statistical output[cite: 17, 22]. [cite_start]Dependencies include `spacy`, `scipy`, and the relevant spaCy language models[cite: 19, 22].

# Limitations

[cite_start]The analysis is limited by the relatively small sample size of the song lyrics[cite: 16, 22]. [cite_start]Future research could include larger corpora or different genres to determine if these correlation strengths generalize across entire languages or remain specific to the selected musical texts[cite: 15, 22].
