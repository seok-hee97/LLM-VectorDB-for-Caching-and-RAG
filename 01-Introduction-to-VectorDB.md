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


