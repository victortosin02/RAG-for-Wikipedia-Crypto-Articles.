Large language models are amazing tools that can help humans obtain answers to questions, summarize extensive texts, translate documents from one language to another, and help us code, among others.
Retrieval-augmented generation (RAG) is an AI framework that has two main objectives: Improve the quality of responses generated by connecting the model to an external source of knowledge and ensure that users have access to the model's sources so you can fact-check its answers for accuracy.

With RAG, we can also ensure that the large language model has access to proprietary data by connecting it to custom sources of data from where it can retrieve information.
The dataset contains a collection of crypto-related articles obtained from Wikipedia. It contains articles about cryptocurrencies, exchanges, companies, facts, and relevant people in cryptocurrency history.

The whole essence of this project is to provide the LLM model updated information about any questions asked on Cryptocurrencies. The information are not static as we have in a traditional LLM but rather due to the connection of the model to an information, it updates the model with up-to-date information about questions asked. 

In this notebook, I will implement a retrieval-augmented generation system for an LLM using the Wikipedia Crypto Articles.

Before I get started with the project, l have to install some relevant packages. These are:

• Chromadb: An open-source embedding database that allows us to plug LLMs to knowledge bases. It allows us to store and query embeddings and their metadata.

• LangChain: A framework that allows us to develop several applications powered by LLMs.

• Sentence Transformers: A framework that provides an easy method to compute dense vector representations for sentences, paragraphs, and images by leveraging pre-trained transformer models.

• bitsandbytes: A library designed to optimize the training and deployment of large models through 4-bit quantization of the model's weights, reducing memory footprint and enhancing memory efficiency.
