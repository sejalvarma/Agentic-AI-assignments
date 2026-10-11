# HR Policy Assistant – RAG Chatbot using n8n

## Project Overview

The **HR Policy Assistant** is an AI-powered chatbot built using n8n and Retrieval-Augmented Generation (RAG). It answers questions about employee leave, attendance, working hours, and workplace policies using a predefined HR policy document.

Instead of relying only on the LLM's general knowledge, the chatbot retrieves relevant information from the knowledge base to generate policy-based responses.

## Objectives

- Build a conversational AI application using n8n.
- Retrieve HR policy information from a predefined document.
- Generate embeddings and store them in a vector store.
- Use an AI Agent to answer user questions based on retrieved information.
- Reduce unsupported answers by identifying information missing from the policy.

## Technologies Used

- **n8n Cloud** – Workflow automation and AI orchestration
- **Google Drive** – HR policy document storage
- **OpenAI Chat Model** – AI response generation
- **OpenAI Embeddings** – Text embedding generation
- **Vector Store** – Semantic search and document retrieval

## Workflow Architecture

The project consists of two workflows:

### 1. Document Ingestion

Google Drive → Read HR Policy → Load Document → Split into Chunks → Generate Embeddings → Store Vectors

### 2. Question Answering

Chat Trigger → AI Agent → HR Policy Search Tool → Retrieve Relevant Information → Generate Response

## Knowledge Base

The chatbot uses a sample HR policy document covering:

- Annual leave and sick leave
- Leave application and approval procedures
- Attendance and working hours
- Late arrival and attendance corrections
- Remote work and overtime
- Unpaid leave and employee responsibilities

## Key Features

- Conversational question answering
- Semantic document retrieval
- Policy-based responses
- Handling of missing information
- Separate document ingestion and question-answering workflows

## Testing

The chatbot can be tested with questions such as:

- How many annual leave days are available?
- How early must annual leave be requested?
- Who approves annual leave?
- How many sick leave days are provided?
- Can unused annual leave be carried forward?

When information is not specified in the knowledge base, the chatbot is instructed to respond:

> I couldn't find this information in the provided HR policy.

## Expected Outcome

The project demonstrates how RAG can be used to build a domain-specific chatbot that retrieves information from documents and generates answers grounded in the available knowledge base.

**Note:** The HR policy is fictional and intended for academic demonstration only.
