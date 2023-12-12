# Generative_AI
Certainly! Here's a detailed set of instructions for the README file:

### Generative_AI_task(Prompt_Engineering.ipynb)

### Personalized Study Plan Generator using OpenAI GPT-3

This Python script utilizes OpenAI's GPT-3 engine to generate personalized study plans for students based on a set of provided parameters. The study plan is designed to address individual academic requirements while aligning with each student's unique needs and aspirations.

### Installation

Make sure to install the OpenAI Python library. You can use one of the following methods:

1. **Install the latest version:**
    ```bash
    pip install openai --upgrade
    ```

2. **Install a specific version (e.g., version 0.28):**
    ```bash
    pip install openai==0.28
    ```

3. **Run the migration command for version 1.0.0:**
    ```bash
    openai migrate
    ```

### Usage

1. **Set Up Your API Key:**
    - Replace `'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'` in the code with your actual OpenAI GPT-3 API key.

2. **Define Student Information:**
    - Edit the `student_info` dictionary with relevant information about the student, such as name, age, academic level, major subjects, etc.

3. **Run the Script:**
    - Execute the script, and it will generate a personalized study plan based on the provided information.

4. **Example Usage:**
    ```python
    # Set your OpenAI GPT-3 API key
    openai.api_key = 'YOUR_OPENAI_API_KEY'

    # Define student information
    student_info = {
        "name": "John Doe",
        "age": 18,
        "current_academic_level": "High School",
        "major_subjects": ["Math", "Science"],
        "academic_performance": "Transcript data...",
        "learning_style": "Visual",
        "extracurricular_activities": ["Chess Club", "Debate Team"],
        "objectives_and_challenges": "Preparing for SAT",
        "aspirations": "To become a physicist",
        "api_key": "YOUR_OPENAI_API_KEY"
    }

    # Generate the personalized study plan
    result = generate_personalized_study_plan(student_info)

    # Display the generated study plan
    print(result)
    ```

### Important Note

Ensure that you comply with OpenAI's use case policies and guidelines when using the GPT-3 engine. It's recommended to review the [OpenAI documentation](https://beta.openai.com/docs/) for the latest information and updates.




/////////////////////////////////////////////////////////////////////////////PDF_SUMMARIZER//////////////////////////////////////////////////////////////////////////////////////////////////////////////////






Sure, here's a basic README template for your code:

```markdown
# LangChain Summarizer

## Overview
The LangChain Summarizer is a Python tool designed to summarize the content of books, leveraging natural language processing and machine learning techniques. The code includes functionality to process various book file types, cluster and summarize their content, and generate a cohesive final summary.

## Installation
To use the LangChain Summarizer, you need to install the required dependencies. You can install them using the following commands:

```bash
pip install langchain
pip install python-dotenv
pip install pypdf
pip install openai
pip install tiktoken
```

Additionally, to use the LangChain Summarizer, you need to obtain an OpenAI API key. Set up a `.env` file with your OpenAI API key:

```dotenv
OPENAI_API_KEY=your_actual_api_key
```

## Usage

### Example Usage

```python
# Import necessary modules
import os
from dotenv import load_dotenv
from langchain_summarizer import generate_summary

# Load environment variables
load_dotenv()

# Provide the OpenAI API key
openai_api_key = os.getenv('OPENAI_API_KEY')

# Example usage with a sample book file
book_path = "/path/to/your/book.pdf"
with open(book_path, 'rb') as uploaded_file:
    summary = generate_summary(uploaded_file, openai_api_key, verbose=True)
    print(summary)
```

## Functions

### `generate_summary(uploaded_file, openai_api_key, num_clusters=11, verbose=False)`

This function takes a book file, OpenAI API key, and optional parameters to generate a summarized output.

## License
This project is licensed under the [MIT License](LICENSE).
```

Please note that you should replace the placeholder text with the appropriate details for your project. Additionally, make sure to update the license information accordingly.
