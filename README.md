# Using-RAG-to-Automate-Emergency-Healthcare-QA-Process
This repo displays code from a University of Chicago MS-ADS Capstone project where we utilized RAG to answer questions on
emergency visit physician notes.



Problem statement
There is a program called MIPS that aims to improve the quality of emergency health care. The current program requires a lot of man-hours
and is very costly/error prone. This project aims at automating some parts of the QA program through RAG.

Data description
Data is HIPAA-compliant emergency visit data. There are about 10,000 visits in total.

Approach/Methodology
Our team utilized a hybrid search agentic-rag architecture. The hybrid search capability in Pinecone allowed us to filter the context per visit. The agent allowed us to utilize md.calc for more information regarding the specific healthcare question (i.e. what qualifies for high probability of pulomonary embolism?") in order to reduce hallucination.

Results
We automated three different components of the MIPS program and saw 92-96% accuracy across 25 different test visits.


Tech stack
Langchain, Pinecone, OpenAI, Tavily

