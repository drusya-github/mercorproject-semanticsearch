# AI Semantic Search


## Project Description

The **basic idea** of the project is to find the **most similar search results to user queries**. 

We will develop a search engine that encodes the user's query into a vector and searches for similarity within a body of text. 
___
## Index 
| S.no | Section                      |
| ---- | ---------------------------- |
| 1.   | [Technologies Used](#technologies-used )       |
| 2.   | [ Important Installations](#important-installations) |
| 3.   |  [ An Overview](#an-overview)            |
| 3.   |  [ Important Terms](#important-terms)       |
| 4.   | [ Scope for improvements](#scope-for-improvements)  |
| 5.   | [Reference](#reference)               |


Link to Youtube Explanation: https://youtu.be/OC9-QZ2aY-U

___
## Technologies Used

- **Python** - The programming language (duh!)
- **openai** - used to develop ai and machine learning algorithm tools.
- **pinecone** - A fully managed vector database that makes it easy to add vector search to production apps.
- **Embed Model** - text-embedding-ada-002
___
## Important Installations

- Log into  [https://app.pinecone.io/](https://app.pinecone.io/)  and create pinecone api key and environment.

-  Log into [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys) and create a key and copy the key into notepad immediately.

- Install the datasets and openai and pinecone clients :

```
pip install -U openai pinecone-client datasets
```

___
## An Overview

1. Initialize and set a pinecone index for searching the data.
2. Load the dataset into pinecone. For this, we are loading the first 1000 rows of TREC(text retreival conference) for training.
3. Next, process the text data in batches to create embedding and insert then to pinecone for efficient similarity search. We are processing the text data in batches of 32 at a time.
4. "query" will be used in search engine to find relevant information. Query needs to be embedded.
5. Generate a text-embedding for the query, which is useful for semantic search.
6. Then, the top-n results, that are most similar to the query are retreived.
___
## Important Terms

| S.no | Term            | Meaning                                                                            |
| ---- | --------------- | ---------------------------------------------------------------------------------- |
| 1.   | **Vector Database** | a type of database that stores data as high-dimensional vector.                    |
| 2.   | **openai api key**  | A unique identifier that helps a program access data and share information.        |
| 3.   | **The Embed Model** | Used to convert text into numerical representation that a computer can understand. |
|      |                 |                                                                                    |
___
## Scope for improvements

- try to make a cute, user-friendly interface that will allow users to enter their queries and view the search results.
___
## Reference

| S.no | Link                                                                         | Description                               |     |     |     |
| ---- | ---------------------------------------------------------------------------- | ----------------------------------------- | --- | --- | --- |
| 1.   | [https://docs.pinecone.io/docs/openai](https://docs.pinecone.io/docs/openai) | To get a general overview of the concept. |     |     |     |
___
