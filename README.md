# 4D Demo AI Similarities

A demonstration project showcasing how to use AI-powered vector embeddings to find similar customers in a 4D database application. This project leverages the 4D AI Kit to detect potential duplicate customers based on semantic similarity rather than exact matches.

## 🎯 Overview

This application demonstrates how to use artificial intelligence to identify similar customers in a database by:
- Generating AI embeddings for customer data
- Computing vector similarities to find duplicates
- Providing an intuitive interface for managing customer data and similarity searches

## ✨ Features

### Customer Management
- **AI-Powered Customer Generation**: Automatically generate realistic customer data using AI
- **Customer Creation Form**: Manual customer entry
- **Smart Vectorization**: Convert customer information into AI embeddings for similarity comparison

### Similarity Detection
- **Vector-Based Matching**: Uses cosine similarity to find potential duplicates
- **Configurable Similarity Threshold**: Adjust the sensitivity of similarity detection
- **Batch Processing**: Search similarities across the entire customer database
- **Real-time Results**: Fast similarity calculations with performance metrics

### AI Provider Support
- **OpenAI Integration**: Support for OpenAI's embedding models (for instance text-embedding-ada-002)
- **Ollama Support**: Local AI model support via Ollama (for instance nomic-embed-text)
- **Flexible Configuration**: Easy switching between different AI providers and models

## 🚀 Getting Started

### Prerequisites
- 4D 20 R10 or later
- 4D AI Kit component
- AI Provider access:
  - **OpenAI**: API key for OpenAI services
  - **Ollama**: Local or remote Ollama installation with embedding models

### Installation
1. Clone this repository
2. Open the project in 4D: `4D_Demo_AI_Similarities.4DProject`
3. Run the application
4. Configure your AI provider settings in the application

## 📋 Usage

### 1. Generate Sample Data
- Select your AI provider and embedding model
- Use the AI Customer Generator to create realistic test customers
- The system generates complete customer profiles with names, emails, phones, and addresses
- Monitor progress as customers are generated

### 2. Create Vector Embeddings
- Select your AI provider and embedding model
- Click "Generate Embeddings" to vectorize all customer data
- Monitor progress as embeddings are generated

### 3. Search for Similarities
- Go to the Search Similarities form
- Adjust the similarity threshold (recommended: 90-95%)
- Click "Search similarities" to find potential duplicates
- Review results with similarity scores and customer details

### 4. Manual Customer Entry
- Use the Create Customer form for manual data entry
- New customers are automatically vectorized if embeddings are configured
- Search for similarities before saving

## 🏗️ Technical Architecture

### Core Classes
- **`AI_Agent`**: Base class for AI operations with provider management
- **`AI_Vectorizer`**: Handles text-to-vector conversion using AI embeddings
- **`AI_CustomerGenerator`**: Generates realistic customer data using AI
- **`customerEntity`**: Customer data model with vectorization capabilities
- **`customer`**: DataClass with similarity search algorithms

### Database Structure
- **Customer Table**: Stores customer information and vector embeddings
- **Provider Settings**: AI provider configurations and API keys
- **Embedding Info**: Tracks vectorization status and metadata

## 🤝 Contributing

This is a demonstration project showcasing 4D AI Kit capabilities. Feel free to:
- Fork the repository for your own experiments
- Submit issues for bugs or feature requests
- Share improvements and optimizations

## 📄 License

This project is provided as-is for educational and demonstration purposes.

## 🙏 Acknowledgments

- Built with [4D](https://4d.com) database platform
- Powered by [4D AI Kit](https://github.com/4d/4D-AIKit)
- Uses OpenAI and Ollama for AI embeddings and generative AI
- Demonstrates modern AI integration in database applications

---

**Note**: This project requires valid AI provider credentials and is intended for demonstration purposes. Production use should include additional error handling, security measures, and performance optimizations.
