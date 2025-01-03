# LegalLLM: California Legal Analytics Chatbot

Welcome to **Harvey Specter[LegalLLM]**, an advanced chatbot that provides legal analytics and insights in the US legal domain, particularly for California. This application leverages state-of-the-art AI models to assist users with detailed, precedent-based responses to their legal queries.

---

## Features

1. **Conversational Interface**:
   - Users can interact with the chatbot in natural language.

2. **Legal Query Assistance**:
   - Retrieves and lists two similar cases based on user input.
   - Recommends the most applicable precedent case with a detailed explanation.
   - Predicts likely judgments based on historical case outcomes and precedents.

3. **Persisted Vector Store**:
   - Efficient storage and retrieval of legal case embeddings using Chroma and HuggingFace.

4. **Session Memory**:
   - Maintains chat history for seamless conversational experiences.

5. **Customizable Prompt**:
   - Tailored prompts ensure the chatbot delivers concise and relevant legal information.

---

## Tech Stack

- **Python**
- **Streamlit**: For building the user interface.
- **LangChain**: Framework for conversational AI.
- **HuggingFace**: Embedding generation.
- **Chroma**: Vector database for efficient retrieval.
- **ChatGroq**: High-performance LLM for conversational interactions.

---

## Prerequisites

1. Python 3.8 or later.
2. Dependencies installed via `requirements.txt`.
3. A valid Groq API Key stored in `config.json`:
   ```json
   {
       "GROQ_API_KEY": "your_api_key_here"
   }
   ```

---

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/legal-llm-chatbot.git
   cd legal-llm-chatbot
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Configurations**:
   - Create a `config.json` file in the root directory with your API key.

4. **Run the Application**:
   ```bash
   streamlit run app.py
   ```

---

## File Structure

```
legal-llm-chatbot/
├── app.py              # Main application file
├── config.json         # Configuration file for API keys
├── vector_db_dir/      # Directory for storing vector embeddings
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

---

## Usage

1. Start the application using Streamlit.
2. Enter your legal query in the chat input box.
3. Review the chatbot’s response, which includes:
   - Two similar cases.
   - A recommended precedent case and its relevance.
   - A prediction of the likely judgment outcome.
4. Start a new chat session anytime using the "New Chat" button.

---

## Customization

- **Prompt Template**:
  - Located in `app.py`, the prompt can be modified to adapt the chatbot’s behavior for other domains or jurisdictions.

- **Vector Database**:
  - Update the directory path or database storage mechanism as needed.

---

## Future Enhancements

- Add multi-jurisdictional support.
- Enable integration with external legal databases.
- Provide citation export functionality for retrieved cases.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgments

- The **LangChain** team for their conversational AI framework.
- **Streamlit** for providing an intuitive platform for building web applications.
- The **HuggingFace** and **Chroma** communities for their robust libraries and support.

