This repository provides the complete implementation of a semantic book recommendation system built using large language models (LLMs). The project demonstrates how to combine natural language processing techniques, semantic search, classification, sentiment analysis, and a user-friendly web interface into a cohesive AI-powered application.

The system is structured into five main components:

Data Preparation & Cleaning – The dataset is explored and preprocessed to ensure high-quality inputs for downstream tasks (data-exploration.ipynb). This includes removing inconsistencies, normalizing text, and preparing metadata for use in later stages.

Semantic (Vector) Search – A vector database is created to store book embeddings, enabling the retrieval of items most similar to a user’s query (vector-search.ipynb). For example, the system can return recommendations for prompts such as “a book about a person seeking revenge”.

Zero-Shot Text Classification – Using LLM-based zero-shot classification, books are labeled as fiction or non-fiction without the need for labeled training data (text-classification.ipynb). These labels form a facet that allows filtering recommendations based on genre.

Sentiment & Emotion Analysis – The system applies LLM-driven sentiment analysis to determine the tone of each book description (sentiment-analysis.ipynb). Emotions such as suspense, joy, or sadness are extracted, enabling users to sort recommendations based on mood or emotional impact.

Interactive Web Dashboard – An application built with Gradio (gradio-dashboard.py) provides an intuitive interface where users can search for books, apply filters, and receive recommendations in real time.

The project was developed with Python 3.11 and uses a set of dependencies listed in the requirements.txt file, including pandas, matplotlib, seaborn, langchain, transformers, gradio, and others. The data for this project is sourced from Kaggle, with instructions provided in the repository for downloading and preparing it. An .env file containing an OpenAI API key is required to enable LLM-powered features such as embedding generation, classification, and sentiment analysis.

This end-to-end implementation serves as a practical example of how LLMs and vector databases can be combined to build domain-specific recommendation engines. By integrating semantic understanding, genre classification, emotional tone analysis, and an accessible web interface, it delivers a personalized and engaging book discovery experience.
