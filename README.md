# LLama3.3-RAG  Application using SambaNova the Lightning-fast inference engine

A high-performance RAG (Retrieval-Augmented Generation) application for document chat, built with state-of-the-art components.

## Tech Stack

- **SambaNova**: Lightning-fast inference engine for Llama 3.3
- **Llama Index**: RAG orchestration framework
- **Qdrant**: Vector database for efficient embedding storage
- **Streamlit**: User interface framework

## Prerequisites

- Python 3.11 or later
- Docker (for Qdrant)
- SambaNova API key

## Setup Instructions

1. **Configure SambaNova**
   
   Get your API key from [SambaNova](https://sambanova.ai/) and create a `.env` file:
   ```bash
   SAMBANOVA_API_KEY=<YOUR_SAMBANOVA_API_KEY>
   ```

2. **Launch Qdrant VectorDB**
   ```bash
   docker run -p 6333:6333 -p 6334:6334 \
   -v $(pwd)/qdrant_storage:/qdrant/storage:z \
   qdrant/qdrant
   ```

3. **Install Dependencies**
   ```bash
   pip install streamlit llama-index-vector-stores-qdrant llama-index-llms-sambanovasystems sseclient-py
   ```

4. **Launch Application**
   ```bash
   streamlit run app.py
   ```

## Usage

1. Start the application using the command above
2. Upload your documents through the Streamlit interface
3. Begin chatting with your documents using natural language queries

## Contributing

We welcome contributions! Please:

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to your branch
5. Create a Pull Request

## License

This project is licensed under the MIT License.
# fastest_rag_stack
