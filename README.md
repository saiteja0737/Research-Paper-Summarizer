# Research Paper Summarizer for Literature Surveys
Doing a literature survey means going through dozens of research papers to find which ones are actually relevant to your topic — this can take hours or even days of reading. This tool automates that process by analyzing each PDF, extracting key information, and generating a structured Excel table with a relevance score and color coding so you can instantly see which papers are worth reading in depth.

## What this tool does
- Reads all PDF research papers from a folder
- Extracts key fields: objective, methodology, validation method, standards, limitations and more
- Scores each paper by relevance to your research topic (1-10)
- Generates a color coded Excel table — green (highly relevant), yellow (moderate), red (low relevance)
- Sorts papers from most to least relevant automatically

## How to Use
1. Add your PDF papers to a folder called `papers/` in the same directory as this notebook
2. Update the `research_topic` variable below with your research area
3. Run all cells
4. Check the output Excel file generated in the same directory

## Requirements
- OpenAI API key in a `.env` file
- Install dependencies: `uv pip install pdfplumber pandas openpyxl openai python-dotenv`

---
*Built as a Day 1 extension project for the Udemy course: AI Engineer Core Track — LLM Engineering, RAG, QLoRA, Agents by Ed Donner.*

### Install required libraries
Run the cell below before running the rest of the notebook:
- `pdfplumber` — extracts text from PDF files
- `pandas` — creates and manipulates the data table
- `openpyxl` — creates and formats the Excel output file
- `openai` — connects to the OpenAI API to analyze papers
- `python-dotenv` — securely loads your OpenAI API key from .env file
