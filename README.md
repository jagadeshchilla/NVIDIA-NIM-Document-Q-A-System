# NVIDIA NIM Document Q&A System

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://python.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28%2B-red.svg)](https://streamlit.io)
[![NVIDIA](https://img.shields.io/badge/NVIDIA-NIM-green.svg)](https://nvidia.com)
[![LangChain](https://img.shields.io/badge/LangChain-Community-orange.svg)](https://langchain.com)
[![FAISS](https://img.shields.io/badge/FAISS-Vector%20Store-purple.svg)](https://faiss.ai)

A sophisticated Document Question & Answer system powered by NVIDIA's NIM (NVIDIA Inference Microservices) and LangChain, featuring advanced RAG (Retrieval-Augmented Generation) capabilities for intelligent document analysis.

## 🚀 Project Overview

This project demonstrates the integration of NVIDIA's cutting-edge AI inference services with modern document processing techniques. It provides an interactive web interface for querying US Census documents using advanced language models and vector embeddings.

## 🎯 Key Concepts

### NVIDIA NIM Integration
- **NVIDIA Inference Microservices**: Leverages NVIDIA's optimized inference infrastructure
- **Meta Llama 3.3 70B**: Utilizes the powerful 70-billion parameter language model
- **NVIDIA Embeddings**: High-performance vector embeddings for semantic similarity

### RAG (Retrieval-Augmented Generation)
- **Document Ingestion**: Automated PDF processing and text extraction
- **Text Chunking**: Intelligent document segmentation for optimal retrieval
- **Vector Storage**: FAISS-based vector database for efficient similarity search
- **Context-Aware Responses**: Generates answers based on retrieved document context

### Advanced Features
- **Streaming Responses**: Real-time answer generation with reasoning display
- **Document Similarity Search**: Shows relevant document chunks for transparency
- **Session Management**: Persistent vector store for improved performance
- **Interactive UI**: User-friendly Streamlit interface

## 🛠️ Technical Methods

### 1. Document Processing Pipeline
```
PDF Documents → Text Extraction → Chunking → Embedding → Vector Storage
```

### 2. Query Processing Flow
```
User Query → Vector Search → Context Retrieval → LLM Generation → Response
```

### 3. Core Technologies
- **LangChain**: Orchestrates the RAG pipeline
- **FAISS**: Efficient vector similarity search
- **Streamlit**: Interactive web application
- **PyPDF**: PDF document processing
- **RecursiveCharacterTextSplitter**: Intelligent text segmentation

## 📋 Prerequisites

- Python 3.8 or higher
- NVIDIA API Key
- Internet connection for API access

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Nvidia-NIM-main
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your NVIDIA API key
   ```

## 🎮 Usage

### Basic Chat Interface (app.py)
```bash
python app.py
```
Simple command-line interface for direct interaction with NVIDIA's Llama model.

### Advanced Document Q&A (app1.py)
```bash
streamlit run app1.py
```
Interactive web application with document upload and Q&A capabilities.

## 📊 Features

### Document Analysis
- **Multi-format Support**: Handles PDF documents seamlessly
- **Intelligent Chunking**: Optimized text segmentation (700 chars, 50 overlap)
- **Semantic Search**: Context-aware document retrieval
- **Source Attribution**: Shows relevant document sections

### User Experience
- **Real-time Processing**: Streaming responses with reasoning
- **Interactive Interface**: Intuitive Streamlit-based UI
- **Session Persistence**: Maintains vector store across sessions
- **Performance Metrics**: Response time tracking

## 🔧 Configuration

### Environment Variables
```env
NVIDIA_API_KEY=your_nvidia_api_key_here
LANGCHAIN_API_KEY=your_langchain_key_here
LANGCHAIN_PROJECT=your_project_name
```

### Model Configuration
- **Model**: `meta/llama-3.3-70b-instruct`
- **Temperature**: 1.0 (creative responses)
- **Max Tokens**: 4096
- **Chunk Size**: 700 characters
- **Chunk Overlap**: 50 characters

## 📁 Project Structure

```
Nvidia-NIM-main/
├── app.py                 # Basic chat interface
├── app1.py               # Advanced document Q&A system
├── requirements.txt      # Python dependencies
├── .env                 # Environment configuration
├── us_census/           # Sample documents
│   ├── acsbr-015.pdf
│   ├── acsbr-016.pdf
│   ├── acsbr-017.pdf
│   └── p70-178.pdf
└── README.md            # This file
```

## 🎯 Use Cases

- **Research Assistance**: Query academic papers and reports
- **Document Analysis**: Extract insights from large document collections
- **Knowledge Management**: Build intelligent document repositories
- **Educational Tools**: Interactive learning from educational materials
- **Business Intelligence**: Analyze corporate documents and reports

## 🔍 Sample Queries

- "What are the key demographic trends in the census data?"
- "Summarize the economic indicators mentioned in the documents"
- "What population statistics are available for different regions?"
- "Explain the methodology used in the census collection"

## 🚀 Performance

- **Response Time**: Optimized for real-time interaction
- **Scalability**: Handles multiple documents efficiently
- **Accuracy**: Context-aware responses based on document content
- **Reliability**: Robust error handling and session management

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 🙏 Acknowledgments

- NVIDIA for providing the NIM inference services
- LangChain community for the RAG framework
- Meta for the Llama language model
- Streamlit for the web interface framework

## 📞 Support

For questions and support, please open an issue in the repository or contact the development team.

---

**Built with ❤️ using NVIDIA NIM, LangChain, and Streamlit**