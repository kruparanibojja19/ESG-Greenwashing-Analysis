# ESG Greenwashing Analysis Using Natural Language Processing

## 1. Overview

Corporate Environmental, Social, and Governance (ESG) reports provide
information about companies' sustainability commitments and performance.
However, analyzing these reports manually can be challenging because
they contain large amounts of unstructured text.

This project applies Natural Language Processing (NLP) techniques to
analyze corporate ESG disclosures by examining their semantic similarity
to Sustainable Development Goal (SDG) reference content and the sentiment
expressed in the reports.

The objective is to compare ESG communication across companies and
reporting years and identify patterns that may warrant further
investigation for potential greenwashing.

**Note:** Similarity and sentiment scores alone cannot establish whether
a company has engaged in greenwashing.

## 2. Research Background

This project is based on the methodological approach presented in:

**Kang, H., & Kim, J. (2022).**
*Analyzing and Visualizing Text Information in Corporate Sustainability
Reports Using Natural Language Processing Methods.*

Applied Sciences, 12(11), 5614.

- Research paper: https://doi.org/10.3390/app12115614
- Original GitHub repository:
  https://github.com/llbtl/paper_ssm01

The original study used semantic sentence similarity and sentiment
analysis to examine corporate sustainability reports.

This project adapts that general analytical approach to ESG disclosures,
with a focus on examining patterns that may be relevant to potential
greenwashing.

The original researchers' work is acknowledged as the methodological
foundation for this project.

## 3. Objectives

- Analyze ESG reports from multiple companies and reporting years.
- Examine semantic relationships between report sentences and SDG
  reference content.
- Analyze sentiment patterns in ESG disclosures.
- Compare results across companies and reporting years.
- Explore how NLP-based analysis can support the screening of ESG
  disclosures for further investigation.

## 4. Methodology

The project follows a multi-stage NLP pipeline.

### Step 1: Text Extraction
Extract text from corporate ESG reports and divide it into individual
sentences.

### Step 2: Semantic Similarity Analysis
Use the Sentence Transformers MiniLM model to generate sentence
embeddings and calculate cosine similarity between ESG report sentences
and SDG reference sentences.

### Step 3: Sentiment Analysis
Use DistilBERT-based sentiment analysis to examine positive and negative
sentiment patterns in ESG disclosures.

### Step 4: Score Normalization
Apply min-max normalization to the similarity scores to facilitate
comparison and visualization.

### Step 5: Visualization and Comparison
Visualize and compare semantic similarity and sentiment-related results
across companies and reporting years.

## 5. Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Sentence Transformers
- MiniLM
- DistilBERT
- PyTorch
- Scikit-learn


