GenAI App - AI Code Reviewer
This is a Streamlit web application that uses Google Generative AI (Gemini-Pro) to review Python code, identify issues, and suggest improvements.

Features
Accepts Python code input via a text area.
Provides detailed code reviews with suggestions and corrected snippets.
Displays warnings and error handling with retries for API requests.
Prerequisites
Python installed on your system.
A valid Google Generative AI API Key.
Installation
Clone the repository:

git clone https://github.com/yourusername/genai-code-reviewer.git
cd genai-code-reviewer
Install dependencies:
Ensure you have pip installed, then run:

pip install -r requirements.txt
Set up secrets:
Create a secrets.toml file in the .streamlit directory with your Google API key:

GOOGLE_API_KEY = "your-api-key-here"
Usage
Run the application:

streamlit run app.py
Enter your Python code in the provided text area.

Click "Review Code" to receive feedback on bugs and suggestions.

Requirements
The following packages are necessary to run the app:

streamlit
google-generativeai
(Dependencies are listed in requirements.txt)

File Structure
📂 project-folder/
   ├── app.py               # Main Streamlit application
   ├── requirements.txt     # Python dependencies
   
Notes
The app uses exponential backoff to handle API errors gracefully.
API Key should be kept secure and not shared publicly.
