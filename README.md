# Misogyny-Repeated-and-Reposted
A computational discourse analysis of misogynistic memes using Speech Act Theory, NLP, and multimodal alignment metrics. This repository provides the notebooks developed to analyze How Toxic Memes Enact Gendered Ideology through Multimodal Speech Acts.

# Research Questions
Sub-RQ1: How do toxic memes enact gendered ideologies as speech acts?

Analyzed locutionary (content), illocutionary (intent), and perlocutionary (audience reaction) levels using:

Close reading of a MAMI dataset meme.

Sentiment analysis (VADER) of Reddit comments via PRAW.

Sub-RQ2: What linguistic patterns sustain gendered ideologies?

NLP pipeline: Keyword extraction, verb collocate analysis, and subtype-based frequency (spaCy, pandas).

Focus on performative speech acts (e.g., insults, directives) and gendered referents ("woman," "bitch").

Sub-RQ3: How does text-image alignment affect rhetorical force?

CLIP (ViT-B/32) for semantic alignment.

SIGLIP for visual explicitness scoring.

Qualitative validation of "amplify" (overt) vs. "obscure" (ironic) memes.

# Methodology Overview
Tools & Libraries
Data Collection: PRAW (Reddit API), MAMI dataset (SemEval-2022 Task 5).

NLP: spaCy (lemmatization, tokenization), VADER (sentiment), 4CAT (word trees).

Multimodal Analysis: CLIP (cosine similarity), SIGLIP (explicitness scores).

Visualization: Matplotlib, Seaborn.

Pipeline
Sub-RQ1:

Reddit comment scraping → VADER sentiment → Bar charts.

Sub-RQ2:

Text preprocessing → Frequency/collocate analysis → Heatmaps.

Sub-RQ3:

CLIP/SIGLIP scoring → Correlation tests → Manual validation.

# Reproducing the Analysis
Dependencies
pip install praw spacy matplotlib seaborn transformers torch pandas
python -m spacy download en_core_web_sm

Data
MAMI Dataset: Test split (1000 memes + metadata CSV) from SemEval-2022 Task 5.

Reddit Data: Collected via PRAW (sample code in notebook).
