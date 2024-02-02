# AtliQ Tees: Talk to a Database

Hey there! Welcome to my AtliQ Tees Talk to a Database project – an exciting journey where I've built a system capable of conversing with a MySQL database using LangChain and Google Palm Language Model (LLM). This system allows users to ask questions in natural language, and it intelligently generates SQL queries to interact with the AtliQ Tees T-shirt store's MySQL database.

## Project Overview

AtliQ Tees is an innovative T-shirt store offering Adidas, Nike, Van Heusen, and Levi's T-shirts. The store's inventory, sales, and discounts data are stored in a MySQL database. In this project, I've developed an end-to-end Question and Answer (Q&A) system that incorporates the following technologies:

- Google Palm LLM
- Hugging Face Embeddings
- Streamlit for User Interface
- LangChain Framework
- ChromaDB as a Vector Store
- Few-Shot Learning

The UI is designed to allow store managers to ask questions in natural language, and the system responds by generating accurate SQL queries and executing them on the MySQL database.

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/codebasics/langchain.git
   ```

2. **Navigate to the Project Directory:**
   ```bash
   cd AtliQ-Tees-Talk-to-a-Database
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Acquire a Google API Key:**
   - Visit [makersuite.google.com](https://makersuite.google.com/) to obtain an API key.
   - Place the key in the `.env` file:
     ```env
     GOOGLE_API_KEY="your_api_key_here"
     ```

5. **Database Setup:**
   - Run `database/AtliQ-Tees-Talk-to-a-Database.sql` in your MySQL Workbench for database setup.

## Usage

1. **Run the Streamlit App:**
   ```bash
   streamlit run main.py
   ```

2. **Explore the Interface:**
   - Ask questions in natural language, and the system will provide answers based on the MySQL database.

## Sample Questions

- "How many total T-shirts are left in stock?"
- "How many T-shirts do we have left for Nike in XS size and white color?"
- "What is the total price of the inventory for all S-size T-shirts?"
- "How much sales amount will be generated if we sell all small size Adidas shirts today after discounts?"

## Project Structure

- **main.py:** The main Streamlit application script.
- **langchain_helper.py:** My creation, housing all the LangChain-related code.
- **requirements.txt:** A list of required Python packages for the project.
- **few_shots.py:** Contains few-shot prompts.
- **.env:** Configuration file for storing the Google API key.
