# LLMs

## Adding Dependencies:

Some dependencies we use `uv` to install:

* `requests`: to fetch the FAQ dataset from internet
* `minsearch`: a simple in-memory search engine for indexing and searching text
* `openai`: OpenAI API client for calling the LLM
* `jupyter`: notebook environment
* `python-dotenv`: load API keys from .env file 

## RAG Helper:

* `ingest.py`: loading data and building the search index
* `rag_helper.py`: the RAG logi (search, prompt, LLM)




