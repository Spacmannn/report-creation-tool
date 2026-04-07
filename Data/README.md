# arXiv Dataset Description

## About
### Source and Provenance
We use the **arXiv Dataset** available on Kaggle:
https://www.kaggle.com/datasets/Cornell-University/arxiv/data

This dataset was originally collected and released by Cornell University and contains information from scientific papers published on arXiv, an open-access repository widely used by researchers.

However, the Kaggle version mainly provides **metadata and abstracts**, not full paper text. We plan to extend this dataset by accessing arXiv Open Access (OA bulk) to download full-text papers (LaTeX/PDF) and convert them into plain text. We will also explore alternative open-access scientific datasets if needed.

### Size and Structure

- 1.7M+ scientific papers
- JSON metadata format

**Key fields**
- `id` – paper identifier
- `authors` – paper authors
- `title` – paper title
- `abstract` – paper summary
- `categories` – research area
- `doi` – digital object identifier
- `journal-ref` – publication info
- `versions` – version history

### Domain
Scientific and academic research papers in STEM fields. 


## Why This Dataset is Suitable

This dataset supports our NLP task with:

- large-scale academic corpus
- real scientific writing examples
- consistent academic language
- open-access and legally usable
- structured metadata for filtering
- full-text papers can be obtained from arXiv OA bulk

It enables analysis of paper structure and writing patterns, which aligns with the project objectives.

## Challenges

### 1. Limited Text
The Kaggle dataset mainly contains abstracts and metadata. Our options:
- Try downloading full papers from arXiv OA bulk and convert LaTeX/PDF to text
- Scrapping from arXiv
- Alternative dataset as last resort

### 2. Large Dataset Size
The dataset contains over 1.7 million papers, which are too large to process. We plan to retrieve random ~10k samples.

### 3. Processing
Plain text papers might not provide structured section labels and require lots of cleaning. We plan to use rule-based section extraction and/or keyword detection

## Dataset Usage in This Project

The dataset will be used to:
- collect full scientific papers
- extract structured sections
- analyze academic writing patterns
- support NLP analysis of scientific reports
