# Graph_RAG
Documents are converted into graph data, stored inside Neo4j, retrieved using graph relationships, and finally used by an LLM to generate the answer.



## Complete GraphRAG Flow

```text
Movie Documents
      ↓
Chunking
      ↓
LLM extracts entities + relationships
      ↓
Neo4j Knowledge Graph
      ↓
User Question
      ↓
Question → Cypher
      ↓
Neo4j retrieves connected facts
      ↓
Retrieved facts + question → LLM
      ↓
Final Answer
```

