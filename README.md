Immigration Rules Assistant App
A powerful and user-friendly web application designed to simplify the complex process of navigating immigration rules. Built for the Rag and Roll Hackathon, this app allows users to upload immigration-related documents, categorize them, and receive precise answers to their questions.

Features
Database Integration: A robust Snowflake database stores and manages uploaded documents.
Document Chunking: Large documents are split into smaller, searchable chunks for better context and accuracy.
Vector Database: Categorizes chunks (e.g., H1 visas, family sponsorship) to enable contextually relevant responses.
User-Centric Design: Users can filter by categories to focus on specific topics of interest.
Real-Time Updates: Upload new documents to keep the app updated with the latest immigration rules.
Streamlit Interface: A clean, intuitive interface for seamless user interaction.
How It Works
Upload Documents: Users upload immigration-related documents into the system.
Categorization: Documents are processed into chunks and categorized into topics like visa types or sponsorships.
Search and Retrieve: Users ask questions and select categories, and the app retrieves precise answers from the vector database.
Customizable Options: Users can filter results based on their needs, ensuring personalized responses.
Technologies Used
Frontend: Streamlit for building the user interface.
Backend:
Snowflake Snowpark for database management.
Custom Python scripts for document chunking and categorization.
Vector Database: Used to embed and retrieve document chunks for efficient search.
Languages: Python (3.8–3.10).
Installation and Setup
Prerequisites
Python 3.8–3.10 installed on your machine.
Snowflake account for database setup.
Steps to Install and Run
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/immigration_rules_assistant.git
cd immigration_rules_assistant
Set up a virtual environment:

bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Set up Snowflake connection parameters:

Add your Snowflake credentials to a .streamlit/secrets.toml file:
toml
Copy
Edit
[general]
account = "<your_snowflake_account>"
user = "<your_snowflake_user>"
password = "<your_snowflake_password>"
role = "<your_snowflake_role>"
warehouse = "<your_snowflake_warehouse>"
database = "<your_snowflake_database>"
schema = "<your_snowflake_schema>"
Run the app:

bash
Copy
Edit
streamlit run streamlit_app.py
Sample Questions to Try
Visa Types: "What is an H1 visa?"
Application Process: "How do I apply for an L1 visa?"
Required Documents: "What documents are needed for family sponsorship?"
Challenges and Learnings
Challenges:

Chunking large documents without losing context.
Efficiently integrating a vector database for accurate retrieval.
Ensuring the app remains intuitive and user-friendly.
Learnings:

Improved understanding of Snowflake’s Snowpark capabilities.
Gained experience in using vector databases for search optimization.
Developed a deeper appreciation for user-centric design in complex workflows.
Future Enhancements
Add multilingual support to handle immigration rules in multiple languages.
Introduce AI-powered insights for more conversational and context-aware responses.
Enable mobile compatibility for easier access on the go.
Provide real-time updates to reflect changes in immigration policies instantly.
Contribution
Contributions are welcome! Feel free to submit a pull request or open an issue for suggestions or improvements.

License
This project is licensed under the MIT License. See the LICENSE file for details.
