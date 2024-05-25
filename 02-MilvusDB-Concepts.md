#### Introduction to Milvus DB

- What is Milvus
Milvus is a specialized database that is built for storing, indexing, and searching vectors.

- Milvus DB Features
  - Open source and commercial
  - Standalone, cluster, and managed (Zilliz Cloud) options
  - Highly scalable for vector storage and search
  - Euclidean distance(L2), inner product(IP) and COSINE metrics
  - Hybrid data storge and search
  - Access with SDKs(Python, Node.js, Go, Java)

#### Milvus Architecture


- Milvus architecture(simplified)

![img](fig/Milvus-arrchitecture.png)

link : [Milvus Architecture Overview](https://milvus.io/docs/architecture_overview.md)


#### Collections in Milvus

- Databases in Milvus
  - Each Milvus instance can manage mulitple databases(max: 64)
  - Default databases is "default"
  - A database is a container for data
  - RBAC implemented by database
  - Multitenancy option


- Collections in Milvus
  - A Milvus collection is like a table in traditional databases
  - Has schema that defines fields for data storage
  - 