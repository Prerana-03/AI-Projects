# YouTube Lecture Summarizer (Beginner)

This project automates the summarization of YouTube technical talks or lectures. It extracts the video transcript and uses OpenAI's API to generate concise summaries, allowing you to get the key points of a video without needing to watch it in full.

## Project Overview

This tool:
1. Extracts the video ID from a YouTube URL using a regex pattern.
2. Uses the `youtube-transcript-api` to retrieve the video's transcript.
3. Passes the transcript to OpenAI's GPT API to summarize the content.
4. Outputs a summary with key points from the lecture.

## Project Structure



## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/YouTubeSummarizer.git
    cd YouTubeSummarizer
    ```

2. **Install dependencies**:
    Run the following command to install the required Python libraries:
    ```bash
    pip install -r requirements.txt
    ```

3. **Get an OpenAI API key**:
    - Visit the [OpenAI website](https://beta.openai.com/signup/) and sign up for an API key.
    - Add your API key in the `main.py` script where indicated.

## Usage

1. **Edit the Script**:
    - Open `main.py` and replace the placeholder for `OPENAI_API_KEY` with your actual API key.
  
2. **Run the Script**:
    Use the following command to generate a summary of a YouTube video:
    ```bash
    python main.py
    ```

    The script will prompt you for the YouTube video link and will extract the transcript, summarize it, and output the key points.

3. **Output**:
    The script generates a concise summary of the video's key points.

## Example

1. **Input**:
    - **YouTube Video Link**: Provide the URL of the video you want to summarize (e.g., a technical talk).
  
2. **Output**:
    - **Summary**: A concise summary of the video transcript with the most important key points.

## Libraries Used
- **openai**: For generating summaries of video transcripts using GPT-4.
- **youtube-transcript-api**: For extracting transcripts from YouTube videos.
- **re**: For extracting the video ID using a regular expression.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
