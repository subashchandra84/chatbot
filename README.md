# Chatbot using LLM and langchain framework.
      **Author: Subash Chandra R**
      **Date: 28th Feb,2024**
## Leveraging the OPEN API, and vector DB(PineCone) to store the vectors.
**Pre-req**:
  1) Need to generate a OpenAI API Key
  2) Need to create a Pinecone Vector API Key
  3) Python 3.11 version is req
**Steps**:
  1) Read the input data(Pdf file in our case)
  2) Break the data into chunks(500, we have set as an base)
  3) convert chunks to embeddings(Using OPENAI Embeddings, we can use any but OpenAI Embeddings has an edge)
  4) Instantiate Vector database instance(Pincecone in our case). We can use any vector DB, but one needs to assess the use case
       ![image](https://github.com/subashchandra84/chatbot/assets/43601110/1f981b4f-8f5e-461a-bef6-b695c30cc614)
                                       src:"https://www.datacamp.com/blog/the-top-5-vector-databases"
  6) Perform a cosine similarity search to retrive the results from Vector DB.
  7) Initiate the OPEN AI model "**text-davinci-003**"
  8) Perform QA and cross verify with the target data.
