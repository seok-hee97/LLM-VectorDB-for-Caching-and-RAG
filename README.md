# LLM: VectorDB for Caching and RAG
(LLM Foundations: Vector Databases for Caching and Retrieval Augmented Generation (RAG))


### Scope of the Course
- Vector and Vector search concepts review
- Concepts and Setup of Mulvus DB
- Milbus DB data manipulation and search
- VectorDB as a LLM cache
- VectorDB for Retrieval Augmented Generation (RAG)

### Course Prerequisites
- NLP for Machine Learning
- LLM and Embeddings
- Python, jupyter notebooks, Docker
- LangChain

### Course details

As large language models grow in popularity, the infrastructure to be used around them also becomes vital to reduce costs, generate accurate responses, and improve efficiency. Vector databases play a vital role in several LLM use cases to help alleviate LLM shortcomings, reduce costs and latency. Knowledge of its basics and applications are vital for any engineer building applications with LLMs, and in this course, Kumaran Ponnambalam teaches you the basics of vector databases and how to use them in LLM caching and retrieval-augmented generation (RAG).

Kumaran begins with a discussion on the basics of vector databases and their applications. He then explores specialized databases for storing vectors and uses the Milvus database as the reference example, and demonstrates read and write operations with the Milvus database. Learn how to use vector databases for LLM caching, with an example use case, along with examples of RAG use cases. Finally, Kumaran concludes with a discussion on optimizing vector databases.



#### What is Vector??
A Vector is an object that has both magnitude(size, quantity)   
and direction(line, angle, trend).  

- Examples of Vectors
  - Velocity
  - Momentum
  - Force
  - Weight
  - Temperature

- Vectors in Programming
  - A one-dimensional data structure
  - Homogeneous(has elements of the same type)
  - Defined position for each element
  - Storage/access different from listas and arrays

#### Vectorization in NLP
- ML with Text Data
  - ML algo can only handle numeric data
  - Text data need to be converted to equivalent 
    numeric representations for ML purposes
  - Vectorizeation converts text to numeric values
  - Captures structure and/or semantics of original text

- Vectorization Techniques
  - Bag of Words
  - TF-IDF(text frequency - inverse document frequency)
    - Creats sparse metrics of documents
  - Word embeddings
    - Captures semantic information in vectors
  - Sentence embeddings
    - Popular with large language model(LLM)-baased applcations


#### Vector Similarity search
- Vector Similarity
  - Each vector has a series of data points
  - A sentence can be a vector of its embeddings
  - Similarity measures how close two vector are
  - Distance measures are used to measure similarity
    - Euclidean distance(L2)
    - Inner product(IP)
    - Cosine similarity(COSINE)

- Similarity Search for Text
  - Vectorize strings using any of the vectorization techniques
    - List of strings to search
    - Query string to compare against
  - Compare Vectors using approximate nearest neighbor(ANN) algorithms
  - Use distance mesures with ANN to determine similarity
  - Retrieve top-K results ordered by similarity


#### Vector DataBase
Vector databases are specialized database products    
that are optimized for storage and querying of vector size.   


- Vectore Database Features
  - Support for vector data types
  - Support for regular data types
  - CRUD operations on vector and scalar data
  - Semantic search on vector data


- Vector Database Available.    

||Open source|Commercial|
|------|---|---|
|Specialized Vector database|Milvus,Chroma, Vespa, Qdrant|Pinecone, Weaviate|
|General database support vector search|PostgreSQL, Cassandra, OpenSearch|Elasticsearch, Redis, SingleStore|


#### VectorDB - Analysis

- VectorDB - Advantages
  - Semantic search support(ANN, distance measures)
  - Bulk data loading
  - Indexing
  - Efficient data retrieval
  - Scalability
  - Clustering and fault tolerance

- VectorDB - Shortcommings
  - Limited support for traditional querying
  - Transactinal support
  - Insert Latency when handling large datasets
  - Computationaly expensive for semantic searches
  - Memory intensive
  - Intergrations


Which of the following vectorization techniques create a single vector for a entire string??

Sentence embedding!!


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
