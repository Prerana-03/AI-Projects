# Resume Optimization with OpenAI (Beginner)

This project automates the process of tailoring a resume to different job descriptions using OpenAI's GPT-4 API. It reads a resume in Markdown format, compares it with a given job description, and outputs an optimized resume that better matches the job requirements. The updated resume can be converted to both HTML and PDF formats for easy sharing.

## Project Overview

The resume optimization process involves:
1. **Resume Markdown Input**: Provide a resume in Markdown format.
2. **Job Description Input**: Provide a job description.
3. **OpenAI API Call**: Automatically adjust the resume to better align with the job description.
4. **Output**: Receive an updated resume in Markdown, HTML, and PDF formats.

### Steps:
1. **Resume in Markdown**: Convert your resume to Markdown format (You can easily do this with ChatGPT or manually).
2. **OpenAI API**: Use the GPT-4 model to adapt your resume dynamically based on the job description.
3. **Convert to HTML & PDF**: Use Python libraries `markdown` and `pdfkit` to convert the Markdown resume to HTML and PDF.

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
    - Add your API key in the `main.py` script where indicated.

## Usage

1. **Edit the Script**:
    - Open `main.py` and replace the placeholder for `OPENAI_API_KEY` with your actual API key.
  
2. **Run the Script**:
    Run the following command to generate the optimized resume:
    ```bash
    python main.py
    ```

    The script will prompt you for:
    - **Path to your markdown resume** (e.g., `resume.md`)
    - **Job description** (e.g., `job_description.txt`)

3. **Output**:
    The script generates an optimized resume in Markdown format, and converts it to HTML and PDF formats.

## Example

1. **Input**:
    - **Markdown Resume**: A resume written in markdown (provided in `resume.md`).
    - **Job Description**: A text file containing the job description (provided in `job_description.txt`).

2. **Output**:
    - **Optimized Markdown Resume**: A tailored resume in markdown.
    - **HTML Resume**: The resume in HTML format.
    - **PDF Resume**: The resume in PDF format for sharing.

## Libraries Used
- **openai**: For using the GPT-4 model to rewrite resumes.
- **markdown**: For converting Markdown files to HTML.
- **pdfkit**: For converting HTML files to PDFs.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
