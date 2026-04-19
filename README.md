# Qdrant_Final_Project
A portfolio-ready vector search application, demonstrating everything I learned in the [“Qdrant Essentials”](https://qdrant.tech/course/essentials/) course.

## Task
Build a sophisticated documentation search engine using hybrid retrieval, multivector reranking, and production-quality evaluation.

## Quick start

1. Create a `.env` file in the root directory with the following content:

```text
# Qdrant environment variables
QDRANT_URL=http://qdrant:6333   # URL of the local Qdrant instance (do not change)
QDRANT_API_KEY=                 # Qdrant local instance API key (not used; leave blank)

# Hugging Face Token
HF_TOKEN=                       # HugginFace access token used to load models from the Hub (use your own)

# KaggleHub
KAGGLEHUB_CACHE="/workspace/app/datasets"
```
