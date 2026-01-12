<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Build a RAG API with FastAPI

**Project Link:** [View Project](http://learn.nextwork.org/projects/ai-devops-api)

**Author:** Deepak Tiwari  
**Email:** imdeepaktiwari08@gmail.com

---

![Image](http://learn.nextwork.org/restful_gray_jolly_salak/uploads/ai-devops-api_g3h4i5j6)

---

## Introducing Today's Project!

In this project, I built a Retrieval-Augmented Generation (RAG) API using Python and FastAPI, which can answer questions based on custom knowledge stored by the user. The API uses a vector database (Chroma) to store semantic embeddings of knowledge and retrieves relevant information at query time. This project demonstrates how to combine API development with AI-powered semantic search to build intelligent backend systems.  ￼


### Key services and concepts

### Challenges and wins

### Why I did this project

---

## Setting Up Python and Ollama

In this step, I installed Python and set up a virtual environment for the project. I also installed Ollama and downloaded the required language model. These tools are needed to build and run the AI-powered DevOps API and to generate responses using a RAG-based approach.

### Python and Ollama setup

![Image](http://learn.nextwork.org/restful_gray_jolly_salak/uploads/ai-devops-api_i9j0k1l2)

### Verifying Python is working

### Ollama and tinyllama ready

Ollama is a tool that runs AI language models locally. I downloaded the TinyLLaMA model because it is lightweight and works well on local machines. It helps my RAG API generate answers from the retrieved knowledge without using external cloud services.

---

## Setting Up a Python Workspace

In this step, I'm setting up... I need it because..In this step, I created a project folder and set up a Python virtual environment. I installed all required dependencies needed to build and run the AI DevOps RAG API in an isolated and organized workspace.

### Python workspace setup

### Virtual environment

A virtual environment is an isolated Python setup for a project. I am using it to manage dependencies separately and avoid conflicts with other Python projects on my system.

### Dependencies

FastAPI is used to build the API, Uvicorn runs the server, ChromaDB stores and retrieves vector embeddings, and Ollama runs a local language model for generating AI responses.


![Image](http://learn.nextwork.org/restful_gray_jolly_salak/uploads/ai-devops-api_u1v2w3x4)

---

## Setting Up a Knowledge Base

In this step, I created a knowledge base by adding DevOps content and converting it into vector embeddings using ChromaDB. This allows the RAG API to search and retrieve relevant information when a user asks a question.

### Knowledge base setup

![Image](http://learn.nextwork.org/restful_gray_jolly_salak/uploads/ai-devops-api_t1u2v3w4)

### Embeddings created

In this step, I created a knowledge base by adding DevOps content and converting it into vector embeddings using ChromaDB. This allows the RAG API to search and retrieve relevant information when a user asks a question.

---

## Building the RAG API

In this step, I am building a RAG (Retrieval-Augmented Generation) API using FastAPI. I created API endpoints that allow users to add new knowledge and query existing data from the knowledge base. FastAPI is used to expose these endpoints and handle HTTP requests efficiently. This step is important because it connects the vector database and the language model, enabling the system to retrieve relevant information and generate meaningful responses through an API

### FastAPI setup

### How the RAG API works

My RAG API works by..My RAG API retrieves relevant data from ChromaDB using embeddings and then uses the Ollama language model to generate an answer. The main components are FastAPI, ChromaDB, Ollama, and Uvicorn.

![Image](http://learn.nextwork.org/restful_gray_jolly_salak/uploads/ai-devops-api_f3g4h5i6)

---

## Testing the RAG API

In this step, I am testing my RAG API using Swagger UI to verify that the /query endpoint returns correct answers from the knowledge base.

### Testing the API

### API query breakdown

I queried my API by running the command... The command uses the POST method, which means... The API responded with{"answer":"Yes, I can provide the answer:\n\nThe Kubernetes is a container orchestration platform used to manage containers at scale. It provides a set of tools, resources, and APIs for managing, deploying, and running applications in distributed systems. Kubernees is the name of this platform."}% 

![Image](http://learn.nextwork.org/restful_gray_jolly_salak/uploads/ai-devops-api_g3h4i5j6)

### Swagger UI exploration

Swagger UI is an interactive API documentation tool provided by FastAPI. I used it to test my RAG API endpoints and verify that they return correct responses in real time

---

## Adding Dynamic Content

In this project extension, I am adding a new /add POST endpoint to my RAG API. This endpoint allows new content to be dynamically added to the knowledge base through the API, instead of manually editing files or re-running scripts.

When new data is added, it is immediately converted into vector embeddings and stored in ChromaDB. This enables the RAG system to retrieve the latest information in real time.

Overall, this enhancement makes the RAG API more flexible, scalable, and production-ready, as it supports real-time knowledge updates similar to modern production APIs.




### Adding the /add endpoint

![Image](http://learn.nextwork.org/restful_gray_jolly_salak/uploads/ai-devops-api_w9x0y1z2)

### Dynamic content endpoint working

---

---
