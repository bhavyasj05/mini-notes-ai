
---

## 2️⃣ `notes.md` (VERY IMPORTANT) – 10 minutes

This shows **your thinking** (interviewers read this carefully).

Paste this:

```md
## Backend Design
I used FastAPI because it provides fast development, built-in request validation, and automatic API documentation through Swagger.

## Database Schema
I used SQLite for simplicity and local storage.  
The notes table contains:
- id (primary key)
- title
- content
- embedding (stored as BLOB)

Embeddings are stored directly to avoid recomputation during search.

## AI Search Logic
When a note is created, its content is converted into a vector embedding using a sentence-transformers model.  
During search, the query is embedded and cosine similarity is computed against all stored embeddings.  
Results are sorted by similarity score.

## Trade-offs
- Linear scan instead of vector indexing (acceptable for small datasets)
- No authentication due to time constraints
- Simple frontend for faster delivery
