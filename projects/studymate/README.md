# StudyMate

Ask questions about your own lecture notes and get answers that come only from those notes, with citations. If the answer is not in the notes, StudyMate says so instead of guessing.

## How it works
Retrieval-augmented answering, built without an AI model so it runs in the browser:
1. Notes are split into paragraphs.
2. Paragraphs and the question become TF-IDF vectors.
3. Paragraphs are ranked by cosine similarity.
4. If the best score is under a threshold, the app declines. Otherwise it quotes the most relevant sentences and shows citation chips with the full source paragraph.

A built-in **Test accuracy** tab runs 8 questions (6 answerable, 2 out of scope) and reports how often the right source was found and how often it correctly declined.

## Run
Open `index.html`. Upload `.txt` or `.md` files, or paste text. Notes stay in your browser (`localStorage`).

## Limits and next steps
- Keyword-based retrieval misses synonyms. A next step is sentence embeddings, or a language model that rewrites the retrieved passages into a fluent answer while keeping the citations.
- PDF and slide upload would need a parser.
