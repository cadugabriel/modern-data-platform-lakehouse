# modern-data-platform-lakehouse
Exemplo prático de uma arquitetura moderna funcionando
```mermaid
flowchart TD

A[Event Generator Python]
B[Kafka Event Stream]
C[Spark Streaming]
D[Bronze Layer Delta]
E[Silver Layer Clean Data]
F[Gold Layer Aggregated]
G[Analytics / BI]

A --> B
B --> C
C --> D
D --> E
E --> F
F --> G
