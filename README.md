# Question-Answering-PDF-Chatbot
A chatbot build using Langchain, OpenAI and CromaDB


This Repository consist of code for chatbot build using Langchain, openAI GPT model and Embedding DB to answer questions on Uploaded PDF


There are Three phases in building this project

Phase-1:
 Create indexes for textbook/PDF file you would like to ask questions on 
 
 The index.py file creates a index of textbook using croma Embeddings DB using Langchain Loader and textsplitter 
 
Phase-2:
 Create Q&A conversation
 
 Create openAI embeddings for existing indexed data from chromaDB, 
 Use conversationalBufferMemory to store the history of chat conversation and
 use ConversationalRetrievalChain tool from Langchain to initiate QA LLM from OpenAI 

Phase-3:
  Create a chatbot UI around it using Gradio app framework using gradio blocks

Run the APP using command 
```console
python bot.py
```

You can directly upload the book into the bot in the interface


