# Episodic Memory
Represents recent events

```json
{
  "event": 3538,
  "timestamp": 12345,
  
  "actor": 24263,
  "action": 47473,
  "target": 5837,
  "relation": 25,
}
```

Infrastructure:
- PostgreSQL
- MongoDB

# Semantic Memory

Stores concepts, relationships, actions and relations. Knowledge stored here represents what the neural network knows about the environment.

```js
let entities = [
];
let actions = [
    {
        "id": 463,
        "label": "rotation"
    },
];
let relations = [
];
```

Infrastructure:
- Neo4j

# Associative memory

Vectorization of the semantic memory

Infrastructure:
- FAISS
- Qdrant
- Milvus
- DINOv2