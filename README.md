# Resume_Screening_App
An intelligent resume ranking system that automatically analyzes and scores resumes based on job requirements using AI. Built with Streamlit and powered by LLM for accurate candidate matching.
Features

    Automated Resume Analysis: Process multiple resumes (PDF, DOC, DOCX) simultaneously
    AI-Powered Matching: Advanced matching against job requirements using LLM
    Parallel Processing: Fast processing with multi-threading support
    Interactive UI: Clean, modern interface built with Streamlit
    Detailed Analytics:
        Match scoring
        Experience analysis
        Location mapping
        Contact information extraction
    Export Options: Download results in CSV or Excel format

🚀 Getting Started
Prerequisites

    Python 3.10 or higher
    Groq API key (for LLM access)

Installation

    Clone the repository:

git clone https://github.com/yourusername/resume-ranker.git
cd resume-ranker

    Create and activate a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

    Install required packages:

pip install -r requirements.txt

Configuration

    Create a .env file in the project root:

GROQ_API_KEY=your_api_key_here

💻 Usage

    Start the Streamlit app:

streamlit run app.py

    Open your browser and navigate to http://localhost:8501

    Follow these steps in the UI:
        Enter your API key
        Upload resume files (PDF, DOC, DOCX supported)
        Enter the job description
        Click "Start Processing"
        View results and download reports

📁 Project Structure

resume-ranker/
├── app.py              # Streamlit interface
├── resume.py           # Core resume processing logic
├── requirements.txt    # Project dependencies
├── .env               # Environment variables (create this)
└── README.md          # This file

📦 Dependencies

    streamlit: Web interface
    pandas: Data processing
    PyPDF2: PDF file processing
    python-docx: Word document processing
    langchain: LLM integration
    groq: AI model access

🛠️ Development
Add New Features

    Fork the repository
    Create a feature branch:

git checkout -b feature/your-feature-name

    Make changes and commit:

git commit -m "Add your feature"

    Push and create a pull request

Run Tests

python -m pytest tests/

🔍 Sample Output

The system generates a DataFrame with the following columns:

    S.No
    Name
    Experience (Years)
    Location
    Email
    Phone
    Match Score
    File
