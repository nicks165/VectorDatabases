# VectorDatabases Summary:
The code provides a quantitative analysis of six vector databases, including Pinecone, Weaviate, Supabase (PGVector), Zilliz, LanceDB, and Chroma. I also performed Qualitative analysis. I explore each database's feature set, strengths, and weaknesses, comparing them based on performance, scalability, ease of use, and compatibility with different programming languages. 

For the quantitive aspects, I conducted the largest dataset recorded analysis on these databases. Using a dataset of size 35M million, I evaluated these databases on insert speed, semantic query latency, conditional query latency, and individual insert.


Overall, Pinecone was the best performing taking everything into account. Pinecone was the easiest to operationalize and scale to 35M. Zilliz performed best for insert throughout, owing to its differentiated query and index node distribution. Weaviate was always a consistent close contender for each aspect of the workload analysis. However, its and Zilliz’s reliability is a cause for concern. Supabase offered a seamless onboarding, but its vector operations capabilities powered by the PGVector extension were not up to par for an enterprise use case. I could not complete the workload analysis for Supabase due to errors and crashes.

ChromaDB and LanceDB doesn’t have a managed service. LanceDB is more an OLAP Database however it has a huge search and hybrid search latency even when ran locally. Chroma is an in memory database and it only persists data on exit. 

In terms of workload analysis, Pinecone and Weaviate were found to be the most efficient in terms of query response time and throughput, while Supabase was lagging. Zilliz showed promising results regarding query response time but lacked in throughput. 

Qualitative analysis revealed that Pinecone and Weaviate had the most user-friendly interfaces and comprehensive documentation, while Zilliz had more complex interfaces and less comprehensive documentation. Supabase (PGVector) had a simple interface but needed more documentation. 

In terms of features, Pinecone and Weaviate had the most advanced features, such as automatic indexing and search relevancy ranking, while Zilliz, Chroma DB and LanceDB had more limited features. Supabase (PGVector) had a good set of features but needed advanced functionalities. 

Overall, Pinecone and Weaviate emerged as the top performers in both workload analysis and qualitative analysis, while Zilliz, Chroma DB and LanceDB had some limitations regarding features and documentation. Supabase (PGVector) showed potential but lacked advanced functionalities and documentation. 
