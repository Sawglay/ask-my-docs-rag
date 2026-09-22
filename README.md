# Ask My Docs — RAG Document Q&A

A Python project for asking questions about a collection of Markdown documents. It uses retrieval-augmented generation (RAG): find relevant passages first, then give those passages to a language model to produce an answer with source file names.

> **Status:** README-first project. The application code and example documents have not been added yet. The commands below describe the planned CLI and will work after the listed files are implemented.

## Project goal

Make a small, understandable document assistant that can answer questions about notes, manuals, or other documents I am allowed to use. The first version will run in the terminal and support Markdown files. It is designed as a learning project, not as a production service.

## Planned workflow

1. Put Markdown files in `data/books/`.
2. Load and split each document into smaller passages.
3. Generate embeddings and store the passages in a local Chroma database.
4. Search that database for passages relevant to a question.
5. Ask an OpenAI chat model to answer using those passages and display the source file names.

**Planned stack:** Python, LangChain, Chroma, and the OpenAI API.

## Planned project layout
