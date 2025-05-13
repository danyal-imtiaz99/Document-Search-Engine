# Building a Document Search Service with Java, GCP, DevOps & AI

## Overview
An intelligent system enabling users to upload documents, extract AI-powered insights, and perform advanced content searches. This application combines Java development with cloud infrastructure and machine learning capabilities.

## Tech Stack
- **Core**: Java 17, Spring Boot 3.2
- **Storage**: PostgreSQL (metadata), Google Cloud Storage (documents)
- **Intelligence**: Google Cloud Natural Language API
- **Infrastructure**: Docker, GitHub Actions, Google Cloud Run

## Current Status
This project is actively evolving with several exciting features in development:
- Semantic search capabilities
- Custom document classification models
- Real-time collaboration features
- Enhanced metadata extraction

## Architecture

```mermaid
graph TD
    A[Upload Service] --> B[Document Parser]
    B --> C[AI Analysis]
    A --> D[Cloud Storage]
    C --> E[Metadata Store]
    D --> F[Search Engine]
    E --> F
    
    classDef primary fill:#4285F4,stroke:#0D47A1,color:white
    classDef storage fill:#34A853,stroke:#0D652D,color:white
    classDef processing fill:#FBBC05,stroke:#E37400,color:white
    
    class A,F primary
    class D,E storage
    class B,C processing

## Getting Started
> Setup instructions coming soon as we stabilize the initial architecture
