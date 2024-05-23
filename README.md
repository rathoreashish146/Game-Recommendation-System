# Game Recommendation System

## Introduction

The Game Recommendation System leverages state-of-the-art techniques such as Retrieval Augmented Generation (RAG) and Large Language Models (LLMs) to provide tailored game suggestions to users. By utilizing natural language processing and advanced machine learning algorithms, this system enhances the gaming experience by delivering personalized recommendations.

## Objective

The primary objective of this project is to build a cutting-edge game recommendation system that utilizes state-of-the-art techniques such as RAG and LLMs. By harnessing the power of natural language processing and advanced machine learning algorithms, the system will deliver tailored game suggestions to users, enhancing their overall gaming experience.

## Key Features

1. **Personalized Recommendations**: Analyze user preferences, gaming history, and other relevant factors to generate personalized game recommendations.
2. **Retrieval Augmented Generation (RAG)**: Combine retrieval-based methods with generative models to retrieve relevant information and generate contextually rich recommendations.
3. **Large Language Models (LLMs)**: Use pre-trained LLMs to understand and process natural language queries, enabling intuitive and conversational user interactions.
4. **Scalability and Performance**: Design to scale efficiently to handle large volumes of user data and provide real-time recommendations with low latency.
5. **User-Friendly Interface**: Feature a user-friendly interface that allows users to explore and discover new games, providing rich metadata and interactive features.

- **Data Collection and Preparation**: 
  - **Data Source**: Steam Games Dataset from Fronkon Games hosted on Hugging Face, which includes comprehensive information on over 85,000 games.
  - **Data Cleaning and Preprocessing**: Handle missing values, select top 100 games based on average playtime, and prepare the dataset for model training.


## System Architecture

### Backend

### Data Preparation Pipeline

1. **Dataset**: Source game data and load it into the system for processing.
2. **Load Data/Content**: Initial processing of game data.
3. **Text Chunks**: Divide data into manageable text chunks for embedding generation.
4. **Embeddings**: Convert text chunks into vector embeddings using pre-trained models.
5. **Build Semantic Index**: Use embeddings to build a semantic index for efficient similarity search and retrieval.
6. **Knowledge Base**: Store the semantic index in a knowledge base for query processing.

### Frontend

### Query and Response Pipeline

1. **User**: Submits a query to the system.
2. **Query**: Convert the user query into a query embedding.
3. **Query Embedding**: Match against the semantic index in the knowledge base.
4. **Ranked Result**: Retrieve and rank information based on relevance.
5. **LLama2**: Process ranked results to generate a coherent response.
6. **Response**: Deliver the final response to the user.

## Tech Stack

### Programming Language
- **Python**: Chosen for its simplicity, extensive libraries, and strong community support, making it ideal for implementing machine learning and data processing tasks.

### Key Libraries and Frameworks

1. **LangChain**: Integrated with LLama2, focusing on linguistic processing tasks such as tokenization, parsing, semantic analysis, and other natural language processing operations.
2. **Flask**: A lightweight web framework for developing the frontend web application interface.
3. **Meta Llama2**: The specific large language model used for processing and generating responses based on user queries.
4. **Pinecone**: A vector database for storing and querying embeddings or vector representations of game data, suitable for similarity search and recommendation systems.


### Real-Time Use Video

Watch our model demonstrating real-time usage of the Game Recommendation Chatbot ![image](https://github.com/rathoreashish146/Game-Recommendation-System/assets/117078265/65185c9d-1b8f-483a-a0ec-31d054be83d7)


### Architecture Flow Chart

![image1](https://github.com/rathoreashish146/Game-Recommendation-System/assets/117078265/0e1073ee-dbd0-456d-956a-724b60281b6c)

![image2](https://github.com/rathoreashish146/Game-Recommendation-System/assets/117078265/4689b8b4-7f3a-4574-8b1e-a0f63ae9b298)



## Future Work and Improvements

1. **Incorporate User Feedback**: Implement mechanisms to collect and analyze user feedback to refine and improve the recommendation algorithm.
2. **Logging and Monitoring**: Set up comprehensive logging and monitoring to track performance and optimize efficiency.
3. **Enhanced Personalization**: Integrate advanced features to tailor recommendations based on user preferences and historical interactions.
4. **Expand Game Database**: Continuously update the game database with the latest releases and a broader variety of genres.
5. **Cross-Platform Integration**: Enable functionality across web, mobile, and gaming consoles.
6. **Real-Time Recommendation Updates**: Implement real-time updates based on trending games and user behavior patterns.
7. **Natural Language Understanding Improvements**: Enhance capabilities to handle more complex and nuanced queries.
8. **Advanced Analytics and Reporting**: Develop tools for insights into user behavior, popular games, and system performance.
9. **Community Features**: Introduce user reviews, ratings, and social sharing to create an interactive environment.

## License

This project is licensed under the MIT License.

## Contact

For any questions or suggestions, please contact Ashish at rathoreashish146@gmail.com.

## How to Run

1. Clone this repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run the Flask web application using `python app.py`.
4. Access the chatbot interface through your web browser.
