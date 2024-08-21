---
title: "AI Project RAG Movie Recommender"
date: 2024-03-15
categories:
  - AI
tags:
  - Data Science
---

Leveraged Google's open-source Gemma model to design and implement a personalized movie recommendation engine, enhancing user experience through tailored content.

Integrated MongoDB for vector-based database management, significantly improving the system's recommendation accuracy and performance.

Tech Stack
MongoDB: Connect to clusterA Python library for interacting with MongoDB that enables functionalities to connect to a cluster and query data stored in collections and documents. MongoDB also support vector database store and has tutorial on how to define vector search pipeline. Also, converting from python dataframe to json-like collection in MongoDB is easy process.

Pandas: Data preparation in python dataframe

Hugging Face Accelerate: Abstracts the complexity of writing code that leverages hardware accelerators such as GPUs. Accelerate is leveraged in the implementation to utilise the Gemma model on GPU resources.

Hugging Face Transformers: Access to a vast collection of pre-trained models

Hugging Face Sentence Transformers: Provides access to sentence, text, and image embeddings.

utilized Google open source model Gemma, embedding to create RAG system with mongoDB

What's Next
The choice of your LLM will change the setup of the code. Google Colab is able to fit Gemma-2B with Tesla V4. To run it locally, llama-cpp-python supports users to use LLM without beast machines.

Integrate in a bigger software by writing a web server using FASTAPI. Host the LLM on cloud. store newer data to database.


![image](https://github.com/user-attachments/assets/45834c7a-6bca-4db9-80ff-6f7b3bc6d041)
![image](https://github.com/user-attachments/assets/4c2100ed-3e0b-4ff6-8a97-4d4c22169fa1)

code -> [Notebook](https://github.com/weibb123/RAG_movie_recommender/blob/main/RAG_system.ipynb)


