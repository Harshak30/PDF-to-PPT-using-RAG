# PDF Chunking and Retrieval

## Overview
This project enables efficient processing and retrieval of PDF document content by breaking it into smaller sections, generating embeddings, and storing them in Pinecone for fast similarity-based searches.

## Process Workflow

### 1. **PDF Chunking**
- Breaks the PDF document into smaller sections or chunks.
- Chunking is based on predefined criteria such as number of characters, bytes, or logical sections like headings and paragraphs.

### 2. **Tag Matching Using LLM**
- Each chunk is processed by a **Large Language Model (LLM)** to generate relevant tags.
- These tags help in categorizing and improving document retrieval.

### 3. **Embedding Generation**
- **SentenceTransformers** are used to generate embeddings for each chunk.
- Embeddings represent the meaning of the content as numerical vectors for efficient retrieval.

### 4. **Storing Results in Pinecone**
- Generated embeddings and associated metadata (tags, text, etc.) are stored in **Pinecone**.
- Pinecone allows for quick retrieval of document chunks based on similarity searches.

### 5. **Slide Generation**
- Users provide titles and subtitles for slides.
- The system retrieves relevant content from Pinecone.
- Titles and associated content are automatically added to the slides.

## Key Benefits
- **Efficient Document Processing**: Breaks down large PDFs into manageable sections.
- **Enhanced Searchability**: Tags and embeddings enable semantic search.
- **Automated Slide Creation**: Generates slides with retrieved content.
- **Scalable Storage**: Uses Pinecone for fast and efficient retrieval.

## Conclusion
This project provides an end-to-end pipeline for structuring, processing, retrieving, and presenting PDF content efficiently using LLMs, embeddings, and vector databases.

