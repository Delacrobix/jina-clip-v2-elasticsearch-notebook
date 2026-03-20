## Ingest Pipeline

```mermaid
flowchart TB
    A[Image] --> B[Jina CLIP v2] --> C[Embedding] --> D[(Elasticsearch)]
```

## Search Pipeline

```mermaid
flowchart TB
    A[Text Query] --> C[Jina CLIP v2]
    B[Image Query] --> C
    C --> D[Embedding] --> E[(Elasticsearch)] --> F[Results]
```
