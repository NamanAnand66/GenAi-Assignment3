# DeepGraph RAG-Pro: Advanced Knowledge Intelligence System

DeepGraph RAG-Pro is a state-of-the-art Retrieval-Augmented Generation (RAG) platform designed for high-precision document intelligence. It combines traditional vector search with Knowledge Graph semantics, neural reranking, and query expansion to provide accurate, context-aware responses using local LLMs.

## 🚀 Key Features

- **Hybrid Retrieval Pipeline**: Seamless integration of BM25 (keyword-based) and FAISS (vector-based) search for robust document retrieval.
- **GraphRAG Capabilities**: Leverages structural knowledge relationships to answer complex queries that traditional RAG might miss.
- **Neural Reranking**: Utilizes Cross-Encoder models to re-evaluate and prioritize the most relevant contexts.
- **HyDE (Hypothetical Document Embeddings)**: Enhances retrieval accuracy through query expansion and hypothetical response modeling.
- **Local-First Architecture**: Powered by Ollama, ensuring data privacy by running models like DeepSeek and Qwen locally.
- **Interactive UI**: A polished Streamlit-based interface with real-time streaming and document management.
- **Dockerized Deployment**: Fully containerized environment for consistent setup across different infrastructures.

## 🛠️ Technology Stack

- **LLM Engine**: [Ollama](https://ollama.ai/) (DeepSeek-R1, Qwen)
- **Frameworks**: LangChain, LangGraph, Streamlit
- **Vector DB**: FAISS
- **Models**: 
  - Embeddings: `nomic-embed-text`
  - Reranker: `cross-encoder/ms-marco-MiniLM-L-6-v2`
- **Orchestration**: Docker & Docker Compose

## 📋 Prerequisites

- [Docker](https://www.docker.com/) and Docker Compose
- [Ollama](https://ollama.ai/) installed and running on the host (if not using the containerized Ollama service)

## ⚙️ Installation & Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/NamanAnand66/GenAi-Assignment3.git
   cd DeepSeek-RAG-Chatbot
   ```

2. **Configure Environment**
   ```bash
   cp env.example .env
   # Edit .env with your specific configurations
   ```

3. **Deploy with Docker**
   ```bash
   docker-compose up --build
   ```

4. **Access the Application**
   Open your browser and navigate to `http://localhost:8501`.

## 📖 Usage

1. **Upload Documents**: Use the sidebar to upload PDF, DOCX, or TXT files.
2. **Configure Settings**: Toggle RAG features like HyDE, Neural Reranking, or GraphRAG based on your requirements.
3. **Query**: Ask complex questions about your data and receive structured, cited responses.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue for feature requests and bug reports.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
*Developed by N Sai Akhil © 2025*
