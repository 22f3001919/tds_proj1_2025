# Agenda

## 1. Source data
 - [ ] Get course data from github (hot tip - dont scrape, just use the markdown)
 - [ ] Get discourse data using API (hot tip - do not scrape the HTML, use the json response)
## 2. Preparing the data
 - [ ] Convert all materials to markdown

> [! Note] Hot tip: Use the LLM to convert the image to a text description and then use the description in the markdown of the post.

- [ ] Create embeddings for all text data
> [! Note] Hot tip: Use npz (a highly compressed numpy array store) to efficiently store the embedding vectors.
- [ ] Chunk appropriately (with overlaps). Overlaps of content help with context accuracy.

## 3. Create the application

- [ ] Create fastapi application (vercel vs render / huggingface)
- [ ] Incorporate the RAG retrieval and chat completion mechanism

