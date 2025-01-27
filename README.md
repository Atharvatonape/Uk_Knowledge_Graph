
# Knowledge Graph on UK Politics

This repository contains a collection of Jupyter Notebooks aimed at building a **Knowledge Graph** on UK politics. The project involves extracting, processing, and linking political entities (e.g., politicians, parties, events, and organizations) using various Natural Language Processing (NLP) and Named Entity Recognition (NER) techniques. The final goal is to generate a structured knowledge graph that can represent relationships within the UK political landscape.

---

## Project Structure

The notebooks are organized sequentially to reflect the workflow of building the knowledge graph. Each notebook tackles a specific part of the process.

### 1. **Downloading Tweets (`1_Downloading_Tweets.ipynb`)**
   - Automates data collection from Twitter using the Twitter API.
   - Focused on extracting tweets related to UK politics (e.g., hashtags, keywords like #UKPolitics, #Brexit).
   - Covers:
     - API authentication.
     - Fetching tweets and storing them for further analysis.
     - Preprocessing raw text data for NLP tasks.

### 2. **Corpus Construction (`2_Spacy_Corpus_Wiki.ipynb`)**
   - Demonstrates how to build a custom corpus from Wikipedia pages on UK politics.
   - Covers:
     - Scraping and cleaning data about UK political entities (e.g., politicians, political parties, laws, events).
     - Preparing data for training and analysis using SpaCy pipelines.

### 3. **Rule-based Matching (`3_Rule_Based_Matching.ipynb`)**
   - Implements rule-based matching techniques using SpaCy.
   - Identifies key phrases and structures related to UK politics, such as party names, parliamentary terms, and government bodies.
   - Useful for extracting information that doesn't require machine learning.

### 4. **Rule-based NER (`4_2_Rule_Based_NER.ipynb`)**
   - Builds upon rule-based matching to perform Named Entity Recognition specific to UK politics.
   - Extracts entities like:
     - Politicians' names (e.g., Boris Johnson, Keir Starmer).
     - Political organizations (e.g., Labour Party, Conservative Party).
     - Dates and locations related to political events.

### 5. **Custom NER (`5_Custom_NER.ipynb`)**
   - Trains a custom NER model tailored to UK politics.
   - Includes:
     - Annotating data with political entities.
     - Training a SpaCy NER model for domain-specific tasks.
     - Fine-tuning the model for accuracy in extracting political entities.

### 6. **Entity Linking (`6_Entity_Linking.ipynb`)**
   - Links recognized entities to external knowledge bases like Wikidata or DBpedia.
   - Resolves ambiguities (e.g., distinguishing between "Johnson" as a person and "Johnson" as a place).
   - Adds context to extracted entities, enriching the knowledge graph.

### 7. **Coreference Resolution (`7_Spacy_Conference_Resolution.ipynb`)**
   - Resolves pronouns and other references in political texts (e.g., speeches, tweets, or articles).
   - Ensures entities are consistently referred to throughout the corpus, improving the quality of the knowledge graph.

---

## Final Output

The final knowledge graph represents relationships between key political entities, such as:
- **Politicians** (e.g., Boris Johnson, Rishi Sunak).
- **Parties** (e.g., Labour, Conservative).
- **Events** (e.g., elections, Brexit negotiations).
- **Organizations** (e.g., Parliament, think tanks).

The knowledge graph can be queried to uncover insights, such as:
- Connections between politicians and policies.
- Trends in political discourse on social media.
- Relationships between events and their stakeholders.

---

## Prerequisites

- Python 3.8+
- Jupyter Notebook
- Required Libraries:
  - `spacy`
  - `tweepy`
  - `pandas`
  - `networkx` (for creating the graph)
  - `matplotlib` (for visualizing the graph)
---

## Applications

This project has applications in:
- **Political Analysis**: Understanding relationships between entities in UK politics.
- **Media Monitoring**: Tracking political discourse on platforms like Twitter.
- **Knowledge Representation**: Building a structured dataset for political events and entities.
- **NLP Research**: Training domain-specific NER models for political text analysis.

---

## Contributions

Contributions are welcome! You can:
- Add new features or improve existing ones.
- Report bugs or suggest enhancements.
- Submit pull requests for review.

