#Finance Domain-Specific FAQ Chatbot with Knowledge Graph Integration using MeTTa

## Project Overview
This project is a **Finance Domain-Specific Conversational Chatbot** that integrates MeTTa, Knowledge Graphs, and Retrieval-Augmented Generation (RAG) to provide accurate and contextual responses to financial queries. The chatbot is designed to assist users with financial queries related to loans, credit scores, debt management, legal transparency, and financial literacy. The chatbot integrates **Google Gemini** as a fallback LLM for handling complex queries.

### Key Features:
1. **Knowledge Graph Storage in MeTTa**: Structured financial data is stored and queried directly within MeTTa.
2. **Graph RAG for Retrieval**: Retrieves the most relevant financial data before generating responses.
3. **MeTTa-Python Integration**: Uses a custom Python interface to interact with MeTTa.
4. **Streamlit Frontend**: A simple web-based UI for user interaction.
5. **Google Gemini as Fallback LLM**: If knowledge-based retrieval fails, Gemini generates responses.

## Tech Stack
### Backend:
- **Python (Flask & Streamlit)** (for API and interface)
- **MeTTa** (for storing and querying financial knowledge)
- **Google Gemini** (fallback LLM for additional responses)

### Frontend:
- **React.js** (for the user interface)


## Repository Structure
```
HackIndia-Spark-3-2025---HackStreet/
│
├── finance/                # React.js Frontend
│   ├── src/                # Frontend source code
│   ├── public/             # Static assets
│   ├── package.json        # Project dependencies
│   └── ...
│
├── backend/                # Backend with MeTTa and Streamlit
│   ├── Gem.py              # Main MeTTa integration logic
│   ├── db.metta            # Knowledge Graph stored in MeTTa
│   ├── metastream.py       # Streamlit interface
│   ├── requirements.txt    # Python dependencies
│   └── ...
│
└── README.md               # Project documentation
```

## Setup Instructions

### 1. Clone the Repository
```sh
$ git clone https://github.com/AnupBhat30/HackIndia-Spark-3-2025---HackStreet.git
$ cd HackIndia-Spark-3-2025---HackStreet
```

### 2. Backend Setup
#### Install Dependencies
```sh
$ cd backend
$ pip install -r requirements.txt
```
#### Run the Streamlit App
```sh
$ streamlit run metastream.py
```

### 3. Frontend Setup
#### Install Dependencies
```sh
$ cd ../finance
$ npm install
```
#### Start the React App
```sh
$ npm start
```

## How It Works
1. **User Query Processing**: User inputs a finance-related query via Streamlit.
2. **MeTTa Knowledge Graph Querying**: The backend searches for relevant financial data within `db.metta`.
3. **Graph RAG Retrieval**: If applicable, a retrieval-augmented process fetches structured financial insights.
4. **Response Generation**:
   - If MeTTa has a relevant response, it returns structured information.
   - If not, the system uses **Google Gemini** as a fallback LLM to generate a response.
5. **Frontend Display**: The React.js frontend displays the chatbot response in an interactive UI.

## Technologies Used
- **MeTTa** - Knowledge graph storage and retrieval
- **Google Gemini** - Fallback LLM for response generation
- **Streamlit** - Web interface for chatbot interaction
- **React.js** - Frontend for a seamless user experience
- **Python (Flask/Custom Integration)** - Backend API
- **Graph RAG** - Intelligent retrieval for knowledge-based responses

## Future Enhancements
- Expand the knowledge graph with more financial data sources.
- Improve the Graph RAG model for better context retrieval.
- Implement user authentication for personalized responses.

---
For any queries, feel free to open an issue on the [GitHub Repository](https://github.com/AnupBhat30/HackIndia-Spark-3-2025---HackStreet).




