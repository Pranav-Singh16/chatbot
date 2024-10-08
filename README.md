# Restaurant Chatbot README

Welcome to the Restaurant Chatbot project! This chatbot enhances your dining experience by providing quick and informative responses to your questions about the restaurant’s menu, reservations, and recommendations. Below, you’ll find detailed instructions on setting up, using, and understanding the chatbot's features.

<div align="center">
  <img src="https://github.com/Pranav-Singh16/chatbot/blob/main/file.JPG" alt="Interacting with Chatbot" width="700" height="400">
</div>

## Table of Contents
- **Installation**
- **Features**
- **Usage**
  -  **User Queries**
  -  **File Queries**
- **Example Interaction**
- **Images**
- **License**

# Installation
To get started with the **Restaurant Chatbot**, follow these steps:

1.**Clone the repository:**
```
git clone https://github.com/your-repo/restaurant-chatbot.git
cd restaurant-chatbot
```

2.**Install required packages:**
```
Install the necessary Python libraries:**
pip install -r requirements.txt
```
3. **Set up environment variables:**
```
Create a .env file in the project directory with the following content:
HUGGINGFACE_API_KEY=your_huggingface_api_key
PINECONE_API_KEY=your_pinecone_api_key
PINECONE_ENVIRONMENT=your_pinecone_environment
```
4.**Run the chatbot:**
You can run the chatbot in Google Colab or any local Python environment that supports the necessary libraries.

# Features
- **Natural Language Processing:** Utilizes Hugging Face models to understand and generate human-like responses.
- **Vector Search Integration:** Leverages Pinecone for efficient document similarity searches, enabling the chatbot to find relevant information quickly.
- **Interactive Query Handling:** Processes both direct user queries and extracts queries from uploaded documents (PDF and DOC formats).
- **User-Friendly Interface:** Built with Gradio, providing an intuitive interface for user interactions.

# Usage
### User Queries
1. **Start the chatbot** in your Python environment.

2. **Type your question** in the text box provided, such as:

- “What’s on the menu today?”
- “Can I make a reservation for 6 PM?”
3. **Submit your query** by pressing the "Submit" button or hitting Enter. The chatbot will analyze your question, perform a similarity search against its knowledge base, and return an appropriate response.

# File Queries

1. **File Upload:**

- Users can upload a PDF document using an upload button.

2. **Text Extraction:**

- The bot reads the document and extracts text, separating lines based on the newline character (\n).
3. **Query Processing:**

- Each line of text is treated as a separate query.
- The bot submits each query individually and retrieves relevant information.

4. **Response Generation:**

- For each query, the bot generates a response based on the most relevant information found.
5. **Display:**

- All responses are displayed in the chat history, allowing users to easily view answers to each question derived from the document.

# Example Interaction
- **User**: "What are the best dishes?"

  **Bot**: "The best dishes mentioned in the hotel restaurant's data are the signature dishes, which are Butter Chicken, Paneer Tikka, Biryani, and Masala Dosa."

- **User uploads a PDF** containing several questions about the menu.

  **Bot**:  " Can the restaurant be booked for private events?' Yes, the restaurant offers private events and booking is not required. You can book private events such as family gatherings and corporate meetings through their website or you can contact their events team at events@indianrestaurant.com for more details."

#Images
### Chatbot Interface
<div align="center">
  <img src="https://github.com/Pranav-Singh16/chatbot/blob/main/interface.JPG" alt="Chatbot Interface" width="700" height="400">
</div>
### User Interaction
<div align="center">
  <img src="https://github.com/Pranav-Singh16/chatbot/blob/main/file.JPG" alt="Interacting with Chatbot" width="700" height="400">
</div>
