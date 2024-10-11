# Automatically Organizing PDFs (Intermediate)

This project automates the organization of research papers on your desktop by analyzing their contents and sorting them into folders based on their topics. It uses text embeddings to group similar articles using clustering algorithms.

## Project Overview
If you have a collection of research papers scattered across your desktop, this tool will analyze each PDF’s content (specifically the abstract) and group similar papers together. The result is that all related papers are organized into separate folders automatically.

### Steps:
1. **Extract Abstract**: Use PyMuPDF to extract the abstract from each research paper.
2. **Generate Embeddings**: Use the sentence-transformers library to convert the abstract into text embeddings.
3. **Clustering**: Group the papers using a clustering algorithm like K-Means based on similarity.
4. **Organize Files**: Create folders for each cluster and move the files into their respective folders.

## Project Structure



## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/OrganizePDFs.git
    cd OrganizePDFs
    ```

2. **Install dependencies**:
    Run the following command to install the required Python libraries:
    ```bash
    pip install -r requirements.txt
    ```

3. **Organize your PDFs**:
    - Place all your research papers (PDFs) into a folder on your desktop.

## Usage

1. **Run the script**:
    Use the command below to run the script:
    ```bash
    python main.py
    ```

    The script will:
    - Extract abstracts from each PDF.
    - Generate embeddings using `sentence_transformers`.
    - Use a clustering algorithm to group similar PDFs.
    - Organize PDFs into folders based on their clusters.

2. **Output**:
    - PDFs are moved into folders representing their topic clusters.

## Example

1. **Input**:
    - PDFs of research papers scattered on your desktop.

2. **Output**:
    - Organised folders with clustered research papers.

## Libraries Used
- **PyMuPDF**: For extracting abstracts from PDFs.
- **sentence_transformers**: To generate text embeddings.
- **pandas**: To handle and store embedding data.
- **sklearn**: To cluster the embeddings using machine learning algorithms like K-Means.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
