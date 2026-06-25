# Vector Index Visual Explorer

An interactive, browser-based visual explainer for common vector index types used in vector databases.

## What it covers

| Index | Description |
|---|---|
| FLAT | Brute-force exact search against all vectors |
| IVF_FLAT | Cluster-based search, only scans the nearest cluster |
| IVF_PQ | Compressed vectors using product quantization |
| IVF_SQ8 | 8-bit scalar quantization, 75% memory reduction |
| HNSW | Graph-based approximate nearest neighbor search |
| DiskANN | RAM + disk hybrid search for billion-scale data |

## How to use

https://imelanthirayan.github.io/vector-search-playground/

## Who is this for

Anyone learning how vector indexes work. The concepts apply to any vector database including Milvus, Weaviate, Qdrant, Pinecone, and others.
