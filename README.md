# Movie Script Analysis with LangChain, ChromaDB, and Gradio

## Overview
This project implements a movie script analysis pipeline using **LangChain**, **SentenceTransformers**, and **ChromaDB**. It allows users to:

- Generate detailed descriptions of a movie’s **characters**, **themes**, and **plot**.
- Encode these descriptions into **vector embeddings** and store them in **ChromaDB collections**.
- Compare a new movie script against existing movies to identify the **most similar ones**.
- Perform a structured **similarity analysis** with step-by-step scoring.
- Interact with the system via a **Gradio web interface** for real-time analysis.

---

## Features
1. **LLM-based Description Generation**  
   Generates character, theme, and plot descriptions using LangChain LLM prompts.

2. **Embedding and Vector Storage**  
   Encodes generated descriptions with `SentenceTransformer` and stores embeddings in ChromaDB collections for fast similarity queries.

3. **Similarity Retrieval**  
   Finds the most similar movies using embeddings from characters, themes, and plots with majority voting.

4. **Step-by-Step Similarity Analysis**  
   Provides a detailed comparison between the user’s script and the most similar movie, including plot structure, characters, themes, and narrative patterns.

5. **Interactive Web Interface**  
   Gradio interface lets users input a movie script and receive a full similarity report.

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/movie-script-analysis.git
cd movie-script-analysis
