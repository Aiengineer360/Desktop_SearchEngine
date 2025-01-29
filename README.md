# Desktop Search Engine Application

## Description
The **Desktop Search Engine Application** is a user-friendly tool that allows users to search through their local document collection efficiently. The application supports multiple file formats including PDF, Word, PowerPoint, Excel, and plain text. It uses a TF-IDF-based search algorithm for ranking documents based on query relevance.

---

## Features
- **File Format Support:** PDF, Word (.docx), PowerPoint (.pptx), Excel (.xlsx), and plain text (.txt)
- **Efficient Search:** TF-IDF-based search for ranking documents
- **Document Management:** Add and remove documents from the search index
- **Pagination:** Navigate through search results with pagination
- **Search Result Highlighting:** Highlights query terms in search results
- **Progress Bar:** Visual feedback during document processing

---

## Installation
1. Clone this repository or download the source code:
   ```bash
   git clone <[repository_url](https://github.com/Aiengineer360/Desktop_SearchEngine)>
   ```
2. Navigate to the project directory:
   ```bash
   cd <main.py>
   ```
3. Install the required Python dependencies:
   ```bash
   pip install nltk PyPDF2 python-docx python-pptx openpyxl
   ```
4. Download the necessary NLTK datasets:
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   ```

---

## Usage
1. Run the application:
   ```bash
   python main.py
   ```
2. **Add Document:** Click on the "Add Document" button to add a document to the search index.
3. **Remove Document:** Select and remove a document from the index using the "Remove Document" button.
4. **Search:** Enter your query in the search box and click "Search" to view relevant results.
5. **Pagination:** Use the "Previous" and "Next" buttons to navigate through search results.

---

## Directory Structure
```
Desktop Search Engine Application
├── search_engine_app.py  # Main application file
├── inverted_index.pkl    # Persistent inverted index file (created after first run)
└── documents.pkl         # Persistent document file (created after first run)
```

---

## Dependencies
- Python 3.x
- NLTK
- PyPDF2
- python-docx
- python-pptx
- openpyxl
- tkinter (comes pre-installed with Python)

---

## How It Works
1. **Document Parsing:** Extracts text from different file types using appropriate libraries.
2. **Text Preprocessing:** Tokenizes, stems, and removes stopwords from the text.
3. **Inverted Index:** Builds an inverted index and calculates TF-IDF scores for efficient document retrieval.
4. **Search:** Processes user queries and ranks documents based on relevance.
5. **GUI:** Provides a user-friendly interface for document search and management.

---

## Troubleshooting
1. **NLTK Errors:** Ensure that you have downloaded the necessary NLTK datasets using:
   ```python
   nltk.download('punkt')
   nltk.download('stopwords')
   ```
2. **Unsupported File Format:** Ensure that the document you are adding is in one of the supported formats.

---

## Contribution
Feel free to fork the project and submit pull requests for enhancements and bug fixes.

---

