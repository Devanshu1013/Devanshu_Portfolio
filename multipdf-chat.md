<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:0A2647,100:205295&height=180&section=header&text=MultiPDF%20Chat&fontSize=38&fontColor=FFFFFF&fontAlignY=40&desc=Conversational%20QA%20Over%20Multiple%20PDF%20Documents&descSize=16&descAlignY=65" width="100%"/>
</p>
<p align="center">
<a href="https://devanshu1013.github.io/Devanshu_Portfolio/">← Back to Portfolio</a>
</p>


## Overview

A conversational Q&A application that lets you chat with multiple PDF documents at once, built with LangChain and Streamlit. Instead of manually searching through documents for an answer, you upload one or more PDFs and ask questions in natural language — the app retrieves the most relevant passages and generates an answer grounded in the actual document content. The app is designed to run locally, with GPU support for faster embedding generation.

**Highlights:**
- Upload and query multiple PDF documents in a single conversation
- Semantic search over document content using deep learning embeddings, not just keyword matching
- Conversational interface that maintains context across follow-up questions
- Can be run locally with GPU acceleration for faster embedding generation

## Background

Searching a single long PDF for an answer is tedious enough — `Ctrl+F` only works if you already know the exact wording used in the document. That problem compounds quickly once there are *multiple* documents to search across, since the answer to a question might be spread across several files, or phrased differently in each. Traditional keyword search also breaks down when a question is phrased differently from the source text, even if the meaning is identical.

MultiPDF Chat addresses this with a retrieval-augmented approach: rather than relying on exact keyword matches, it converts document text into semantic embeddings, so a question and its answer can be matched based on *meaning* rather than shared vocabulary. This makes it possible to ask a natural-language question and get a relevant, grounded answer, even when the source documents use entirely different phrasing than the question itself.

## Methodology

1. **PDF text extraction** — text is extracted from each uploaded PDF
2. **Text chunking** — the extracted text is split into smaller, manageable chunks, since embedding and retrieval work far better on focused passages than on entire documents at once
3. **Embedding generation** — each text chunk is converted into a vector embedding using deep learning-based embedding models, capturing its semantic meaning
4. **Semantic search (vector store)** — the embeddings are indexed for fast similarity search, so that at query time, the chunks most semantically relevant to a question can be retrieved quickly
5. **Conversational retrieval** — when a question is asked, the most relevant chunks are retrieved and passed, along with the conversation history, to a language model that generates a natural-language answer grounded in that retrieved content
6. **Interface** — the entire flow is wrapped in a simple Streamlit app: upload PDFs, ask a question, and get an answer, with the conversation maintaining context across follow-up questions

Because generating embeddings for larger documents can be computationally intensive, the app is designed to be run locally with GPU acceleration, which significantly speeds up the embedding step compared to running on CPU alone.

## Tech Stack

`Python` `LangChain` `Streamlit` `PyPDF2` `Hugging Face Transformers` `FAISS`

---

<p align="center">
<a href="https://github.com/Devanshu1013/Devanshu_Portfolio/blob/main/README.md">← Back to Portfolio</a>
</p>
