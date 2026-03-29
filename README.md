# spacy-stanza-german-ner-comparison
Comparing Named Entity Recognition (NER) on German news titles using spaCy and Stanza

# spacy-stanza-german-ner

Comparing Named Entity Recognition (NER) on German news titles using spaCy and Stanza.

## Project Overview

This project applies and compares two popular NLP libraries — **spaCy** and **Stanza** — for Named Entity Recognition on a dataset of 16,860 German news article titles. The goal is to analyze how each model identifies and classifies entities such as locations, persons, and organizations in German text.

## Dataset

- 16,860 German news article titles from [Jotschi/german-news-titles](https://huggingface.co/datasets/Jotschi/german-news-titles)

## Models Used

| Library | Model |
|--------|-------|
| spaCy  | `de_core_news_sm` (German, small) |
| Stanza | `de` German pipeline with `tokenize` and `ner` processors |

## Methodology

1. **Preprocessing** — Extract titles from dataframe and flatten into a list of strings
2. **spaCy NER** — Apply German spaCy pipeline to all titles
3. **Stanza NER** — Apply German Stanza pipeline to all titles
4. **Comparison** — Compare entity extraction across both models using agreement rate and entity overlap

## Entity Types

| Label | Meaning |
|-------|---------|
| `LOC` | Location |
| `PER` | Person |
| `ORG` | Organization |
| `MISC` | Miscellaneous |

## Requirements

```bash
pip install spacy
pip install stanza
python -m spacy download de_core_news_md
```

## Usage

Open and run the notebook `ner_comparison.ipynb` in Google Colab or Jupyter.

## Results

*Coming soon — comparison of spaCy and Stanza NER outputs on German news titles.*
