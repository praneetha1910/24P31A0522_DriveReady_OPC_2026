# Cafe Napoli – AI Agent
----------------------------
#About the Project

This project is developed as part of my Agentic AI workshop assignment. I chose Cafe Napoli, a real-world cafe business, as my application.

The main idea is to build an AI assistant that can help customers with menu-related questions, item availability, prices and order booking. It also uses a knowledge base to answer questions related to the cafe's business operations.

# Problems Identified

Some of the problems currently faced by Cafe Napoli are:

- Staff management and employee retention.
- Infrastructure and equipment maintenance.
- Lack of proper marketing and online presence.
- No properly documented SOPs for the hot kitchen.

# Technologies Used

- Python
- LangChain
- Groq LLM
- ChromaDB
- Google Colab
- Google Sheets
- LangGraph

# Features

1. **Menu Price Checking:** Customers can ask for the prices of available food and beverages.
2. **Item Availability:** Checks whether a particular item is available on the cafe menu.
3. **Knowledge Search:** Uses ChromaDB to retrieve information about Cafe Napoli and its business challenges.
4. **Order Management:** Collects customer order details and saves confirmed orders in Google Sheets.
5. **Conversation Memory:** Remembers previous messages within the same customer conversation.
6. **Unknown Information Handling:** Avoids making up answers when the required information is not available.

# How It Works

The customer sends a message to the AI assistant. Based on the question, the agent selects the required tool.

- Price questions are handled by the price tool.
- Availability questions are handled by the availability tool.
- Business-related questions are answered using ChromaDB knowledge retrieval.
- Confirmed customer orders are stored in Google Sheets.

InMemorySaver is used to maintain conversation history using separate thread IDs.

# Testing

The agent was tested with different customer queries, including:

- Checking cappuccino prices.
- Asking about Cafe Napoli's operational challenges.
- Testing conversation memory.
- Testing separate customer conversations.
- Asking questions about information not available in the knowledge base.
- Placing a customer order and checking whether it was saved in Google Sheets.

**Test Results:** 6 out of 6 test cases passed after reviewing the responses.

**Pass Percentage:** 100%

# How to Run

1. Open the Day 5 notebook in Google Colab.
2. Install the required Python libraries.
3. Add the Groq API key in Colab Secrets as `GROQ_API_KEY`.
4. Run the notebook cells in order.
5. Connect Google Sheets when authentication is requested.
6. Start testing the Cafe Napoli AI assistant.

# Future Improvements

- Add staff scheduling and management support.
- Include equipment maintenance reminders.
- Create digital SOPs for hot kitchen operations.
- Improve cafe marketing and customer engagement.
- Develop a simple interface for customers and staff.

# Conclusion

Through this project, I learned how to build an AI agent using LangChain, connect different tools, store business information in ChromaDB, and maintain conversation memory.

This project helped me understand how Agentic AI can be used to solve some practical problems in a real-world business like Cafe Napoli.
