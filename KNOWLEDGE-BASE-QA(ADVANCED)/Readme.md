# Knowledge Base Question Answering System (Advanced)

This project implements a Knowledge Base Question Answering (QA) system using a multimodal Retrieval-Augmented Generation (RAG) approach. It searches through a knowledge base to find relevant documents and combines them with the user's query to generate an answer. A user-friendly interface is built using Gradio for easy interaction.

## Project Overview

This project builds upon the multimodal search system to implement a QA system that can answer questions based on document knowledge bases. The core idea is to combine top search results with the user's query and pass them to a multimodal model like Llama 3.2 Vision.

### Steps:
1. **Search the Knowledge Base**: Use a search mechanism similar to the one in Project 4 to retrieve relevant documents.
2. **Combine Search Results with User Query**: After retrieving the top k results, combine them with the user query.
3. **Generate Answers**: Pass the query and search results to a multimodal model for generating the final response.
4. **User Interface**: Create a chat-based interface using Gradio.

## Project Structure



## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/KnowledgeBaseQA.git
    cd KnowledgeBaseQA
    ```

2. **Install dependencies**:
    Run the following command to install the required Python libraries:
    ```bash
    pip install -r requirements.txt
    ```

3. **API Access**:
    - Obtain access to **Together AI's API** for Llama 3.2 Vision. You can get a free API key from [Together AI](https://together.xyz).
    - Add your API key to the `main.py` script in the appropriate section.

## Usage

1. **Prepare the Knowledge Base**:
    - Ensure your documents are stored in a DataFrame, similar to Project 4's multimodal search system.

2. **Run the script**:
    Use the command below to run the QA system:
    ```bash
    python main.py
    ```

3. **User Interface**:
    A Gradio-based user interface will open in your browser, allowing you to interact with the QA system. You can input your query, and the system will search the knowledge base, retrieve relevant documents, and provide an answer.

## Example

1. **Input**:
    - A user asks a question, such as "What are the key points in document X?"

2. **Output**:
    - The system retrieves the most relevant parts of document X and generates an answer based on those.

## Libraries Used
- **PyMuPDF**: For extracting text from PDFs.
- **transformers**: For using multimodal models like Llama 3.2 Vision.
- **pandas**: For storing and processing document embeddings.
- **sklearn**: For performing search operations with clustering algorithms.
- **Gradio**: To create the user interface for the QA system.
- **together/openai**: API access to large multimodal models like Llama 3.2 Vision.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
