# A visual exploration of vectors

A vector embedding encodes an input as a list of floating point numbers.

"dog" → [0.017198, -0.007493, -0.057982, 0.054051, -0.028336, 0.019245,…]

Different models output different embeddings, with varying lengths.

| Model | Encodes | Vector length |
| --- | --- | --- |
| word2vec | words | 300 |
| Sbert (Sentence-Transformers) | text (up to ~400 words) | 768 |
| OpenAI ada-002 | text (up to 8191 tokens) | 1536 |
| Azure Computer Vision | image or text | 1024 |

This repository contains a visual exploration of vectors, using several embedding models.

Go through notebooks in this order:

1. Prepare text vectors: [OpenAI ada-002](prep_openai_ada002.ipynb), [Word2Vec Google News](prep_word2vec_gnews.ipynb)
2. [Vector models](compare_vector_models.ipynb)
3. [Vector distance metrics](vector_distance.ipynb)
4. [Multi-word vectors](movie_vectors.ipynb)
5. [Vector quantization](vector_quantization.ipynb)
6. [Prepare multimodal vectors](prep_multimodal.ipynb)
7. [Explore multimodal vectors](multimodal_vectors.ipynb)
