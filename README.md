

[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://multiplepdfapp.streamlit.app/)

# Document Chat System 📚💬

An intelligent, multi-project document chat system powered by Google's Generative AI and Streamlit. This application allows users to create multiple projects, upload various document types, and engage in AI-assisted conversations based on the content of those documents.

## 🌟 Features

- **Multi-Project Management**: Create and switch between multiple projects
- **Document Processing**: 
  - Support for PDF, DOCX, and TXT files
  - Efficient text extraction and chunking
- **Intelligent Chatbot**:
  - Document-specific answers
  - Similar question detection for faster responses
  - Context-aware AI interactions
- **Multiple Chat Sessions**: Create and manage different chat conversations within each project
- **Modern UI**:
  - Sleek, gradient-style chat bubbles
  - Distinct user and AI icons
  - Fixed chat input for better UX
- **Persistent Storage**: Saves projects, documents, and chat histories

## 🚀 Quick Start

1. **Clone the repository**
git clone https://github.com/yourusername/advanced-document-chat.git
cd advanced-document-chat
text

2. **Set up a virtual environment**
python -m venv venv
source venv/bin/activate # On Windows use venv\Scripts\activate
text

3. **Install dependencies**
pip install -r requirements.txt
text

4. **Set up your Google API Key**
Create a `.env` file in the root directory and add your Google API key:
GOOGLE_API_KEY=your_google_api_key_here
text

5. **Run the application**
streamlit run app.py
text

## 📖 How to Use

1. **Create a New Project**
- Use the sidebar to create a new project
- Enter a unique name for your project

2. **Upload Documents**
- Select your project from the sidebar
- Use the "Upload Documents" expander to add PDF, DOCX, or TXT files
- Click "Process Documents" to extract and index the content

3. **Create a Chat Session**
- Use the sidebar to create a new chat within your project
- Enter a name for your chat session

4. **Start Chatting**
- Select a chat session
- Type your questions in the chat input at the bottom
- Receive AI-generated answers based on your uploaded documents

## 🏗️ Project Structure

advanced-document-chat/
├── streamlit_app.py
├── requirements.txt
├── .env


## 🛠️ Technical Details

- **Frontend**: Streamlit
- **AI Model**: Google's Generative AI (Gemini Pro)
- **Embeddings**: Google Generative AI Embeddings
- **Vector Store**: FAISS for efficient similarity search
- **PDF Processing**: PyPDF2
- **DOCX Processing**: python-docx
- **Text Chunking**: LangChain's RecursiveCharacterTextSplitter

## ⚙️ Configuration

- **Chunk Size**: 1000 characters (adjustable in `CHUNK_SIZE` constant)
- **Chunk Overlap**: 200 characters (adjustable in `CHUNK_OVERLAP` constant)
- **Similarity Threshold**: 0.85 for similar question detection (adjustable in `SIMILARITY_THRESHOLD` constant)

## 🔍 Troubleshooting

- **PDF Extraction Issues**: Ensure PDFs are not encrypted and contain extractable text
- **API Key Errors**: Verify your Google API key in the `.env` file and check your Google Cloud Console for proper permissions
- **Memory Issues**: For large documents, consider adjusting the `CHUNK_SIZE` or processing fewer documents simultaneously

## 📝 License

This project is licensed under the MIT License.

## 📮 Support

For support, please open an issue in the GitHub repository or contact [your-email@example.com].

## 🙏 Acknowledgments

- Google Generative AI team
- Streamlit developers
- LangChain community
- FAISS developers
