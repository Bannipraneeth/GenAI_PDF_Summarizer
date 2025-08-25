✍️ Advanced PDF Summarizer with Gemini
This is a web application built with Streamlit that allows you to summarize PDF documents using Google's Gemini Pro Large Language Model. The app provides a user-friendly interface to upload a PDF, enter a custom prompt, and generate a tailored summary. It also includes advanced controls to fine-tune the summarization process.

✨ Features
Upload PDFs: Easily upload any PDF document directly through the web interface.

Custom Prompts: Guide the summarization process with your own specific instructions (e.g., "summarize for a 5th grader," "extract key financial data").

Selectable Summarization Methods:

Stuff: A fast method that processes the entire document in a single call. Best for smaller documents.

MapReduce: A more robust method that handles large documents by summarizing them in chunks.

Dynamic Controls: Use interactive sliders in the sidebar to adjust the chunk_size and chunk_overlap for more granular control over the text splitting process.

Powered by Google Gemini: Leverages the gemini-1.5-flash-latest model for high-quality, context-aware summaries.

🚀 Setup and Installation
Follow these steps to get the application running on your local machine.

1. Prerequisites
Python 3.8 or higher

pip package manager

2. Clone the Repository
git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
cd your-repo-name

3. Create a Virtual Environment
It's recommended to create a virtual environment to manage project dependencies.

# For Windows
python -m venv venv
venv\Scripts\activate

# For macOS/Linux
python3 -m venv venv
source venv/bin/activate

4. Install Dependencies
Install all the required Python packages using the requirements.txt file.

pip install -r requirements.txt

5. Set Up Environment Variables
You need a Google Gemini API key to run this application.

Create a file named API.env in the root directory of the project.

Add your API key to this file as follows:

GEMINI_API_KEY="your_google_api_key_here"

▶️ How to Run the App
Once you have completed the setup, you can run the Streamlit application with the following command:

streamlit run app.py

This will start a local web server, and the application will open in your default web browser.

🛠️ Technologies Used
Backend: Python

Web Framework: Streamlit

LLM Integration: LangChain

LLM Provider: Google Gemini

PDF Processing: PyPDF

Environment Management: python-dotenv