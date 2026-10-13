# Sentence Embedding Visualization: PCA, t-SNE & UMAP

An exploratory comparison of three dimensionality-reduction methods for visualizing transformer embeddings.

## Technical approach
- SentenceTransformer model: all-MiniLM-L6-v2.
- Inputs: the first 300 tokens from the model tokenizer's vocabulary.
- Saved embedding shape: 300 × 384.
- PCA, t-SNE, and UMAP projections with Plotly scatter plots.

The current code does not use Banking77 or intfloat/e5-large-v2.

## Analytical value
Compare projected structures and communicate how visualization choices affect interpretation. This is a technical exploration rather than a validated customer-intent classifier.

## Explore and run
Open [the notebook](Assignment8.ipynb) in Colab. Install the imported dependencies, including sentence-transformers, and adjust the retained course-template setup paths.

## Limitations and next steps
- Vocabulary tokens may be subword fragments and are not representative customer utterances.
- Tokenizer vocabulary order may vary; save a deterministic sample for reproducibility.
- Dense text labels overlap; use hover labels and show a readable static preview.
- Compare parameter settings and quantify neighborhood preservation before declaring a projection best.
- Projected clusters alone do not validate semantic categories.
- Add a real labeled text dataset if extending this toward customer-intent analysis.

## Project context
Developed by Yiren Shen for Duke's AIPI 590 Explainable AI course.
