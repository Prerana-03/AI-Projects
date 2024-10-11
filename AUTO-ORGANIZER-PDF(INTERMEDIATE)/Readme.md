# Resume Optimization (Beginner)

This project automates the task of adapting your resume to different job descriptions using OpenAI's GPT model. It dynamically rewrites your resume based on the given job description, converting it from markdown to PDF.

## Project Overview
Adapting a resume for each job application can be time-consuming. This Python project leverages OpenAI's GPT API to automate the process, taking a markdown version of your resume and a job description, and outputting an optimized version of the resume.

### Steps:
1. **Markdown Resume**: Start by creating a markdown version of your resume.
2. **Job Description**: Input a job description you'd like your resume to be adapted to.
3. **GPT-4 API**: The script prompts OpenAI's GPT model to rewrite your resume to better match the job description.
4. **Markdown to PDF**: Finally, the script converts the updated markdown resume into HTML and then into a PDF using the `markdown` and `pdfkit` libraries.

## Project Structure



## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/ResumeOptimization.git
    cd ResumeOptimization
    ```

2. **Install dependencies**:
    Run the following command to install the required Python libraries:
    ```bash
    pip install -r requirements.txt
    ```

3. **Get an OpenAI API key**:
    - Visit the [OpenAI website](https://beta.openai.com/signup/) and sign up for an API key.
    - Store the key securely. You'll need it in the script.

## Usage

1. **Edit the script**:
    - Open `main.py` and replace the placeholder for `OPENAI_API_KEY` with your actual API key.
  
2. **Run the script**:
    Use the command below to run the script:
    ```bash
    python main.py
    ```
    The script will ask for the following inputs:
    - **Path to your markdown resume** (e.g., `resume.md`)
    - **Job description** that you want to tailor the resume for.

3. **Output**:
    - After execution, the script generates an optimized resume in both HTML and PDF formats.

## Example

Here’s an example of how the input/output works:

1. **Input**:
    - **Markdown Resume**: You provide your resume in markdown format.
    - **Job Description**: A job description for a software engineer role.

2. **Output**:
    - **Rewritten Markdown Resume**: A markdown file optimized for the job description.
    - **PDF Resume**: The optimized resume as a PDF.

## Libraries Used
- **openai**: For interacting with GPT models via the OpenAI API.
- **markdown**: To convert markdown resumes into HTML.
- **pdfkit**: To convert HTML files to PDFs.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
