# Week 4: Text Analytics & NLP

## Fundamentals of Natural Language Processing- 
- Text Preprocessing & Feature Engineering
- Sentiment Analysis & Text Classification
- Named Entity Recognition (NER) & Part-of-Speech Tagging
- Topic Modeling
- Word Embeddings & Transformer-Based Models
- Introduction to Sequence-to-Sequence Tasks (Summarization, Translation)

## Theory, Courses and Additional Reading

- https://huggingface.co/learn/nlp-course/chapter1/1
- https://www.geeksforgeeks.org/natural-language-processing-nlp-tutorial/?ref=shm
- https://www.geeksforgeeks.org/text-classification-using-scikit-learn-in-nlp/
- https://github.com/mchesterkadwell/named-entity-recognition
- https://arxiv.org/abs/1706.03762
- https://arxiv.org/abs/1411.2738
- https://arxiv.org/abs/1810.04805
  
## Assignments

## Assignment 1: Customer Feedback Insights

### Task: Extract sentiment and key themes from customer feedback to identify common pain points.

### Steps:

- Use a pre-existing dataset (e.g., Amazon Reviews or Trustpilot data from Kaggle).
- Perform basic text preprocessing (lowercasing, stopword removal, tokenization).
- Apply sentiment analysis using a pre-trained model (e.g., Vader, TextBlob, or Hugging Face’s DistilBERT).
- Identify key topics/themes using TF-IDF or Latent Dirichlet Allocation (LDA).
- Generate a simple dashboard (Streamlit/Gradio) to visualize insights.

### Success Criteria:

- The system correctly classifies positive vs. negative feedback.
- Outputs 3-5 key themes from reviews.

## Assignment 2 (Optional/Bonus): Resume Skill Extraction & Job Matching 

### Task: Extract key skills from resumes and match them to job descriptions using basic NLP.

### Steps:

- Use pre-existing resume samples (Kaggle Resume Dataset or generate fake resumes).
- Extract names, job titles, and skills using spaCy’s Named Entity Recognition (NER).
- Compare extracted skills to job descriptions using TF-IDF similarity (no need for complex embeddings).
- Rank resumes based on job relevance (basic score output).

### Success Criteria:

- Outputs top 3 resumes per job posting.
