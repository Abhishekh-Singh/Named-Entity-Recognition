### Problem Statement
Generating and storing structured data from unstructured text.

Task:

Take text data, perform NER and Topic extraction, then store these entities and topics. Entities and topics are considered related if they appear in the same document. We would like to use this graph to determine the relations between topics and entities. You should write a sql query that can return the 100 pairs of entities which are most closely related, and the 100 pairs of topics that are most closely related. You can decide the precise measure of relatedness you use.

### Download Dataset
A corpus of one million news articles can be found at: 
https://research.signal-ai.com/newsir16/signal-dataset.html


### What is the Signal 1M Dataset?
The Signal Media One-Million News Articles Dataset dataset by Signal Media was released to facilitate conducting research on news articles. It can be used for submissions to the NewsIR'16 workshop, but it is intended to serve the community for research on news retrieval in general.

The articles of the dataset were originally collected by Moreover Technologies (one of Signal's content providers) from a variety of news sources for a period of 1 month (1-30 September 2015). It contains 1 million articles that are mainly English, but they also include non-English and multi-lingual articles. Sources of these articles include major ones, such as Reuters, in addition to local news sources and blogs.

### Format

Upon downloading the data, you get a single compressed text file (approximately 1GB in size). You can uncompress it using gzip or zcat, etc. The file is in JSONL format, where each line is a JSON object representing an article. Each article has the following fields:

- id: a unique identifier for the article
- title: the title of the article
- content: the textual content of the article (may occasionally contain HTML and JavaScript content)
- source: the name of the article source (e.g. Reuters)
- published: the publication date of the article
- media-type: either "News" or "Blog"

### General Statistics

Below is a summary of general statistics of the dataset:

- The number of individual unique sources are over 93k
- The dataset contains 265,512 Blog articles and 734,488 News articles
- The average length of an article is 405 words
