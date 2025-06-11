# Agenda

## 1. Source data
 - [x] Get course data from github

> [!NOTE]
> Hot tip: Don't scrape, just use the markdown from https://github.com/sanand0/tools-in-data-science-public/tree/tds-2025-01
 
 - [x] Get discourse data using API

> [!NOTE]
> Hot tip:  Do not scrape the HTML, use the json response

## 2. Preparing the data
 - [x] Convert all materials to markdown

> [!NOTE]
> Hot tip: Use the LLM to convert the image to a text description and then use the description in the markdown of the post.

- [ ] Create embeddings for all text data

> [!NOTE]
> Hot tip: Use npz (a highly compressed numpy array store) to efficiently store the embedding vectors.

- [ ] Chunk appropriately (with overlaps). Overlaps of content help with context accuracy.

> [!WARNING]
> Remember to honour rate limits!

## 3. Create the application

- [ ] Create fastapi application (vercel vs render / huggingface)
- [ ] Incorporate the RAG retrieval and chat completion mechanism

## 4. Deploy the application
- [ ] Deploy the application to vercel (advantage: always up, disadvantage: a little complicated to set up)
- [ ] Deploy the application to render (advantage: easy to set up, disadvantage: not always up)
- [ ] Deploy the application to huggingface/dockerapp (advantage: docker based, high performance; disadvantage: more complex setup)

## 5. Testing and validation
- [ ] Test the application using promptfoo
