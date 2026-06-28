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

## Data Ingestion:

* `sqlite-ingest.ipynb`: fetches data and writes it to a persistent index

### Choosing right tool: 

* `minsearch`: single process, in-memory only, re-indexes on every startup, use when data is small and indexing is fast.
* `sqlitesearch`: separate ingestion and query, file-based (SQLite), open existing index. Use when data is large or ingestion is slow.
* `Elasticsearch`
* `OpenSearch`
* `Qdrant`(vector database)

Architecture stays the same: one process ingests, another queries.

## Agent Frameworks:

* ToyAIKits: course built-in frameworks, easy for study and experimentation

Some others popular frameworks:

* OpenAI Agents SDK
* Pydantic AI
* LangChain/ LangGraph
* Google ADK


