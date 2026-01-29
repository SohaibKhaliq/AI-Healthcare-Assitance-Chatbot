# AI Healthcare Assistance Chatbot 🤖

Welcome to the AI Healthcare Assistance Chatbot repository! This project aims to provide an intelligent, interactive chatbot capable of answering health-related questions by leveraging medical knowledge extracted from uploaded PDF documents.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [License](#license)

## Project Overview

This project uses advanced AI and machine learning techniques to build a chatbot that can assist with health-related queries. The chatbot extracts and analyzes information from medical documents and provides precise and clear answers based on the context provided.

## Features

- **Interactive Health Chatbot**: Ask health-related questions and get responses based on the medical documents.
- **PDF Upload and Processing**: Upload PDF documents containing medical information.
- **Automated Text Extraction**: Extracts text from PDFs and splits it into manageable chunks.
- **Vector Store for Text Embeddings**: Creates and updates embeddings using Google Generative AI.
- **Embeddings Management**: Automatically checks and updates embeddings based on PDF modifications.
- **Streamlit Web Application**: User-friendly interface for interaction.

## Installation

To set up and run this project locally, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/SohaibKhaliq/AI-Healthcare-Assitance-Chatbot.git
    cd AI-Healthcare-Assitance-Chatbot
    ```

2. **Create and Activate Virtual Environment**:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Set Up Environment Variables**:
    - Create a `.env` file in the project root directory.
    - Add your Google API key:
        ```env
        GOOGLE_API_KEY=your_google_api_key_here
        ```

5. **Run the Streamlit App**:
    ```bash
    streamlit run app.py
    ```

## Usage

### Chatbot

1. Navigate to the Chatbot tab.
2. Enter your health-related question in the input field.
3. Get responses based on the medical documents.

### Upload PDFs

1. Navigate to the Upload PDFs tab.
2. Upload one or more PDF documents.
3. Click the "Process" button to extract and update embeddings.

### Dashboard

1. Navigate to the Dashboard tab to view the status of processed files and embeddings.

## Project Structure

├── app.py # Main application file

├── requirements.txt # Required dependencies

├── .env # Environment variables file

├── LLM_DB/ # Directory containing PDF documents

├── faiss_index/ # Directory containing FAISS index and embeddings info

├── README.md # This readme file


## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`
3. Make your changes and commit them: `git commit -m 'Add new feature'`
4. Push to the branch: `git push origin feature-branch`
5. Submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.



---

Thank you for visiting this project! If you find it useful, please give it a star ⭐ on GitHub.
