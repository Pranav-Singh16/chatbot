# Restaurant Chatbot README

Welcome to the Restaurant Chatbot project! This chatbot enhances your dining experience by providing quick and informative responses to your questions about the restaurant’s menu, reservations, and recommendations. Below, you’ll find detailed instructions on setting up, using, and understanding the chatbot's features.

## Table of Contents
- Installation
- Features
- Usage
  -  User Queries
  -  File Queries
- Example Interaction
- Images
- License

# Installation
To get started with the Restaurant Chatbot, follow these steps:

Clone the repository:

bash
Copy code
git clone https://github.com/your-repo/restaurant-chatbot.git
cd restaurant-chatbot
Install required packages:
Install the necessary Python libraries:

bash
Copy code
pip install -r requirements.txt
Set up environment variables:
Create a .env file in the project directory with the following content:

plaintext
Copy code
HUGGINGFACE_API_KEY=your_huggingface_api_key
PINECONE_API_KEY=your_pinecone_api_key
PINECONE_ENVIRONMENT=your_pinecone_environment
Run the chatbot:
You can run the chatbot in Google Colab or any local Python environment that supports the necessary libraries.

# Features
Natural Language Processing: Utilizes Hugging Face models to understand and generate human-like responses.
Vector Search Integration: Leverages Pinecone for efficient document similarity searches, enabling the chatbot to find relevant information quickly.
Interactive Query Handling: Processes both direct user queries and extracts queries from uploaded documents (PDF and DOC formats).
User-Friendly Interface: Built with Gradio, providing an intuitive interface for user interactions.

# Usage
User Queries
Start the chatbot in your Python environment.

Type your question in the text box provided, such as:

“What’s on the menu today?”
“Can I make a reservation for 6 PM?”
Submit your query by pressing the "Submit" button or hitting Enter. The chatbot will analyze your question, perform a similarity search against its knowledge base, and return an appropriate response.

# File Queries
Upload a document (PDF or DOC) using the upload button. The chatbot will read and extract text from the file.

The chatbot will process each line of text extracted from the document as a separate query.

For each extracted query, the chatbot will perform a similarity search to find the most relevant information and generate a response.

The results will be displayed in the chat history, allowing you to view responses to each of your document's queries.

# Example Interaction
User: "What are the best dishes?"

Bot: "Our top dishes include the grilled salmon and the truffle pasta."

User uploads a PDF containing several questions about the menu.

Bot: "From the document, you asked, 'What is the most popular dessert?' The answer is chocolate lava cake."

Images
Chatbot Interface

User Interaction
