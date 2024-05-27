# Vector Databases Best Practices


#### Choose a vector database


- Choosing a VectorDB for Your Use Case
  - Several VectorDB options avilable
    - Cloud vs, standalone, embedded vs. cluster, specialized vs. general
  - Use case decides the choice of the database
    - Storage, scalability, and reliability needs
    - Frequency of hybrid queries
    - OK to store data in the cloud
    - Can provide resoures for local hosting and management?



#### Combine vector and scalar data

- Keep Scalar and Vector Data Together?
  - Specialized vector databases
    - Excellent support for vector search
    - Lack the extensive query capabilities that traditional databases provide
  - Does the use case require hybrid search?
  - Keep scalar and vector data in seperate databases?
  - Choose carefully, since it has significant implications



#### Distance Measure Considerations

- Distance Measure Considerations
  - Vector search will always return hits if recodrs exist in DB
  - Distance/similarity thresholds needed to check if vectors in DB match the vector in query
  - What exactly is similar? Depends on the use case
  - Embedding models and metric type impact similarity thresholds
    - Custom embedding by domain( examples: healthcare, finance)




#### Tune vector DB Performance

- Tuning Vector Search Performance
  - Effectiveness of search depends upon the search data, embedding model, metric type, and thresholds
  - Find the best combination by experimentation
    - Use a good test dataset that matches real-world data
    - Experiemtn with embedding modeling models and metric types
    - Experiment with different distance thresholds to find th optimal value
  - Continue to monitor this performance in production also