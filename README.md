# Transformers for Recipe Generation and Sentiment Classification

`transformer_recipes_imdb.ipynb`

- **Part I** — a GPT (one causal transformer block) trained on the Epicurious recipe dataset to generate recipes, with a temperature study and a comparison against an autoregressive LSTM (coherence, creativity, diversity).
- **Part II** — the same GPT block turned into a binary classifier for IMDB reviews (no pretrained weights), compared with an LSTM classifier.

Hyperparameters: VOCAB_SIZE=10000, MAX_LEN=200, EMBEDDING_DIM=100, N_UNITS=128, VALIDATION_SPLIT=0.2, SEED=42, BATCH_SIZE=32, EPOCHS=20.

The notebook downloads the Epicurious dataset from Kaggle (`hugodarwood/epirecipes`) with `kagglehub` on first run. IMDB comes from `keras.datasets`. In Colab, select a GPU runtime and choose Run all.
