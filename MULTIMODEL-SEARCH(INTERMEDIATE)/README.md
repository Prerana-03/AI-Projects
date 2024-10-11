# Multimodal Search (Intermediate)

This project implements a multimodal search tool that allows users to search both textual and image data simultaneously. It leverages embeddings from both text and images to provide search results that combine the two modalities.

## Project Overview
Multimodal search refers to the ability to retrieve results using more than one form of data—usually text and images. This project creates embeddings for both text and images and allows users to perform a search that combines these modalities to find the most relevant results.

### Steps:
1. **Text Embeddings**: Convert search queries into text embeddings using sentence-transformers.
2. **Image Embeddings**: Convert images into embeddings using a pre-trained image model.
3. **Multimodal Search**: Combine text and image embeddings to perform a search across both data types.

## Project Structure


## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/MultimodalSearch.git
    cd MultimodalSearch
    ```

2. **Install dependencies**:
    Run the following command to install the required Python libraries:
    ```bash
    pip install -r requirements.txt
    ```

3. **Data Preparation**:
    - Prepare your dataset of images and associated text files to test the multimodal search.

## Usage

1. **Edit the script**:
    - Modify `main.py` to add paths to your text and image datasets.
  
2. **Run the script**:
    Use the command below to run the script:
    ```bash
    python main.py
    ```

    The script will ask for a search query and perform a search that takes into account both text and image data.

3. **Output**:
    - The most relevant results based on both text and image modalities.

## Libraries Used
- **sentence_transformers**: For generating text embeddings.
- **torchvision**: For generating image embeddings.
- **pandas**: For handling and storing the embeddings.
- **sklearn**: For combining and searching across text and image embeddings.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
