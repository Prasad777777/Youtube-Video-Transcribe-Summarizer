

# End-to-End YouTube Video Transcription and Summarization App (Powered by Google Gemini Pro)

Welcome to the repository for the End-to-End YouTube Video Transcription and Summarization App!  
This application harnesses the powerful Google Gemini Pro API to automatically transcribe and summarize YouTube videos, offering a quick and effective way to digest lengthy video content.

## ✨ Features

- **Automatic Transcription**: Converts audio from YouTube videos into readable text.
- **Summarization**: Creates clear and concise summaries using advanced NLP models.
- **Simple Web Interface**: Intuitive UI for uploading and managing video links.
- **Highly Scalable**: Built to efficiently process large amounts of video data.

## 📚 Table of Contents

- [Installation](#installation)  
- [Usage](#usage)  
- [Configuration](#configuration)  
- [Architecture](#architecture)  
- [Contributing](#contributing)  
- [License](#license)  

## 🛠️ Installation

Clone this repository:

```bash
git clone https://github.com/yourusername/yt-transcribe-summarizer.git
cd yt-transcribe-summarizer
```

Set up a virtual environment:

```bash
python -m venv venv
source venv/bin/activate    # For Windows: venv\Scripts\activate
```

Install the required Python packages:

```bash
pip install -r requirements.txt
```

Set up your environment variables:  
Create a `.env` file in the project root directory and add your Google Gemini Pro API key:

```makefile
GOOGLE_GEMINI_PRO_API_KEY=your_api_key_here
```

## 🚀 Usage

Launch the web application:

```bash
streamlit run app.py
```

Open your browser and visit:  
[http://localhost:8501](http://localhost:8501)

Upload your video by simply providing the YouTube URL, and the app will automatically:

- Transcribe the video
- Summarize the content
- Display both the transcript and the summary directly in the web interface

## ⚙️ Configuration

You can adjust settings inside the `config.py` file. Key options include:

- `TRANSCRIPTION_SERVICE_URL`: The URL for the transcription service.
- `SUMMARIZATION_MODEL`: Model used for summarization (default is Google Gemini Pro).
- `OUTPUT_DIR`: Directory where generated files will be saved.

## 🏗️ Architecture

The project structure is organized as follows:

- `app.py`: Main application file (Streamlit app).
- `transcription.py`: Handles transcription using Google Gemini Pro API.
- `summarization.py`: Summarizes the transcribed content.
- `config.py`: Configuration and settings.
- `requirements.txt`: Lists all dependencies.
