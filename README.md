<div align="center">
  <h1>🤖 Chatbot Assistant with Airtable Integration</h1>
  <p>An intelligent chatbot assistant that extracts specific user data (name, email, phone number) and seamlessly saves it to Airtable.</p>
</div>

<br/>

## 🎯 About the Project

This project implements a conversational AI agent designed to interact with users and securely gather lead or contact information. By leveraging the OpenAI API for natural language processing, the chatbot efficiently extracts essential details—such as the user's name, email address, and phone number—and automatically logs them into an **Airtable** database using custom function calling.

## 📂 Repository Structure

The core files and directories in this repository are structured as follows:

```text
├── agent-template/          # Frontend/UI template files for the chatbot interface
├── assistant_instructions.py # Contains system prompts and core behavior instructions for the assistant
├── custom_functions.py      # Python functions handling external API calls (e.g., Airtable integration)
├── knowledge.docx           # Knowledge base document used by the assistant for context (RAG)
├── main.py                  # Main execution script and server entry point
├── requirements.txt         # Project dependencies
└── .env                     # Environment variables (needs to be created manually)
```
## 🛠️ Technologies Used
- Programming Language: Python

- AI/LLM Integration: OpenAI API (Assistant API / Function Calling)

- Database/CRM: Airtable API

- Deployment: Linux Server (Ubuntu/Debian) via SSH & nohup

## ⚙️ Environment Variables
Before running the application, you need to create a .env file in the root directory and define the following variables:
```
OPENAI_API_KEY=your_openai_api_key_here
AIRTABLE_API_KEY=your_airtable_api_key_here
```
## 🚀 Installation & Deployment
Follow the steps below to deploy the application on a Linux server:

### 1. Connect to your server via SSH:

```
ssh root@YOUR_SERVER_IP
```
### 2. Clone the repository and navigate into it:

```
git clone [https://github.com/BahadirKarsli/Chatbot-Assistant.git](https://github.com/BahadirKarsli/Chatbot-Assistant.git)
cd Chatbot-Assistant
```
### 3. Install the venv module (if not already installed):

```
sudo apt update
sudo apt install python3-venv
```
### 4. Create and activate a virtual environment:

```
python3 -m venv .venv
source .venv/bin/activate
```
### 5. Install the required dependencies:

```
pip3 install -r requirements.txt
```
### 6. Configure the environment variables:

```
nano .env
# Add your OPENAI_API_KEY and AIRTABLE_API_KEY, then save and exit.
```
### 7. Run the server in the background:

```
nohup python3 main.py &
```

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to submit a Pull Request or open an Issue if you have suggestions for improving the integration or adding new features.
