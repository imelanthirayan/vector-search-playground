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

Open `index.html` in any browser. No server, no install, no build step needed.

Each index page has editable inputs. Change any value and the results update live.

## Stack

- Plain HTML
- Vanilla JavaScript
- Tailwind CSS (CDN)

## Files

```
index.html       Home page with index cards
flat.html        FLAT index demo
ivf-flat.html    IVF_FLAT index demo
ivf-pq.html      IVF_PQ index demo
ivf-sq8.html     IVF_SQ8 index demo
hnsw.html        HNSW index demo
diskann.html     DiskANN index demo
script.js        Shared utilities (cosine similarity, helpers)
```

## Similarity method

All demos use cosine similarity.

```
similarity = dot(A, B) / (|A| * |B|)
```

Vectors are 3-dimensional. All values are editable in real time.

## Who is this for

Anyone learning how vector indexes work. The concepts apply to any vector database including Milvus, Weaviate, Qdrant, Pinecone, and others.
