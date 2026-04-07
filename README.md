# ScholarFlow AI - Generating structured academic papers from informal research notes

Github Repository: https://github.com/Spacmannn/report-creation-tool 

## 1. About
**NLP Tasks**
- Text Generation / Controlled Text Generation
- Summarisation and Content Structuring
- Style Transfer / Paraphrasing: Converting informal or standard language into formal Academic Tone

**Domain**: Academic Research & EdTech

**Use Case**: Assist students and researchers in drafting manuscripts for scientific conferences or journals. 

## 2. Why
**Motivation**: Writing academic papers is a difficult and time-consuming process, especially for non-native English speakers and early-stage researchers. Many begin with informal notes, rough ideas, or experimental results, but struggle to convert them into structured academic writing.

**Problem Solved**:
- Reduces time spent on manual formatting and organizing paper sections according to logical standards.
- Improves linguistic quality for non-native English speakers or those unfamiliar with specialized academic prose.

**Importance**: This project enhances accessibility to academic writing, efficiency and may potentially increase the acceptance rate of papers by ensuring professional presentation.

**Functionality**: The system takes unstructured, note-like input (e.g., research outcomes, bullet points, or informal descriptions) and generates a structured scientific abstract or full paper with formal academic tone and standard section organization.

## 3. Final Product
**Expected System**:  A prototype academic writing generation tool that converts informal research notes into structured scientific text.

**Key Outputs**: 
- Structured abstract or report section
- Formal academic tone
- Coherent and organized scientific writing

**Improvements over existing processes**:
- Reduces Manual Rewriting: Helps users automate structuring of academic text and significantly speed up the drafting process.
- Goes Beyond Standard Grammar Checkers: Unlike tools like Grammarly, which focus on grammar/spelling, this system focuses on structural logic and factual accuracy within the text.


## 4. Data

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

**Domain**
Scientific and academic research papers in STEM fields. 

### Why This Dataset is Suitable

This dataset supports our NLP task with:

- large-scale academic corpus
- real scientific writing examples
- consistent academic language
- open-access and legally usable
- structured metadata for filtering
- full-text papers can be obtained from arXiv OA bulk

It enables analysis of paper structure and writing patterns, which aligns with the project objectives.

### Challenges

**1. Limited Text**
The Kaggle dataset mainly contains abstracts and metadata. Our options:
- Try downloading full papers from arXiv OA bulk and convert LaTeX/PDF to text
- Scrapping from arXiv
- Alternative dataset as last resort

**2. Large Dataset Size**
The dataset contains over 1.7 million papers, which are too large to process. We plan to retrieve random ~10k samples.

**3. Processing**
Plain text papers might not provide structured section labels and require lots of cleaning. We plan to use rule-based section extraction and/or keyword detection

### Dataset Usage in This Project

The dataset will be used to:
- collect full scientific papers
- extract structured sections
- analyze academic writing patterns
- support NLP analysis of scientific reports

## 5. Team Responsibilities
**Linh**
- Data cleaning and section extraction
- Document dataset and experimental results, manage deadlines
- Prepare proposal, report, and presentation

**Igor**
- Design NLP pipeline and modeling approach
- Implement and optimize models
- Guide technical methodology

**Huy**
- Support data scraping/preprocessing
- System evaluation & testing
- Handle deployment or interface (if time allows)

