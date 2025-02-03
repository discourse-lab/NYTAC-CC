# NYTAC-CC: A Climate Change Subcorpus from the New York Times Annotated Corpus

## Overview

NYTAC-CC is a climate change-specific subcorpus extracted from the **New York Times Annotated Corpus (NYTAC)**. It consists of **3,630 XML files**, each representing a full-length news article related to climate change, published between **1987 and 2007**. The corpus was created to facilitate research on climate discourse in traditional news media and supports both **quantitative and qualitative** NLP analyses.

## Corpus Description

- **Source**: Extracted from the **New York Times Annotated Corpus (LDC release)**, which includes 1.8 million articles.
- **Time Span**: 1987-2007
- **Number of Articles**: 3,630
- **Format**: XML files, each corresponding to a single article.
- **Metadata**: Articles include metadata such as publication date, newsroom desk, and manually-annotated topics.

## Corpus Construction

The NYTAC-CC subcorpus was created using a **hybrid retrieval approach** that combines:

1. **Keyword-based filtering**: Identifying climate change-related terms using curated lists of bigrams and keywords.
2. **Supervised classification**: Using an **XGBoost classifier** trained on manually annotated samples to refine the selection and remove false positives.
3. **Validation with ClimateBERT**: Assessing corpus relevance with a climate-specific BERT model to ensure high precision and recall.

## Data Structure

Each XML file contains:

- **Article text**: The full content of a climate change-related news article.
- **Metadata**: Including publication date, author (if available), section, and topic labels.

## Applications

NYTAC-CC can be used for:

- **Climate change discourse analysis** in news media
- **Topic modeling and temporal trend analysis** (e.g., using LDA)
- **Sentiment analysis and stance detection**
- **Supervised learning tasks** for NLP research

## Citation
You can find the full paper in this repository under `NYTAC-CC_paper.pdf`.

If you use NYTAC-CC in your research, please cite:

> Grasso, F., Patz, R., & Stede, M. (2024). NYTAC-CC: A Climate Change Subcorpus based on New York Times Articles. *CLiC-it 2024: Tenth Italian Conference on Computational Linguistics*.

## License

This dataset is made available under the **Creative Commons Attribution 4.0 International (CC BY 4.0) License**.

## Contact

For questions or collaborations, please contact **Manfred Stede** or **Francesca Grasso** at [stede@uni-potsdam.de](mailto\:stede@uni-potsdam.de) or [fr.grasso@unito.it](mailto\:fr.grasso@unito.it).

