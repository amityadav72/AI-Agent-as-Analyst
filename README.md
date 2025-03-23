# AI Analyst Agent using n8n, ChatGPT 40 Mini & OpenAI Embedding 3 Small

## Overview
This repository contains an AI-powered analyst agent built using **n8n**, **ChatGPT 40 Mini**, and **OpenAI Embedding 3 Small**. The agent processes files from **OneDrive**, converts them into **vector data**, and responds intelligently using embeddings. Users can leverage this AI chatbot for various analytical purposes such as **stock analysis, financial insights, data interpretation, and more**.

## Features
- **Automated Data Extraction**: Fetches files directly from OneDrive.
- **Vector Embedding Processing**: Converts extracted data into vectors using OpenAI Embedding 3 Small.
- **Conversational AI**: Uses ChatGPT 40 Mini to provide relevant insights based on embedded data.
- **Stock & Data Analysis**: Users can analyze stock trends, perform financial assessments, and obtain insights on uploaded datasets.
- **Customizable Workflow**: Built with n8n, making it highly flexible and easy to modify.

## Workflow Architecture
1. **File Input**: User uploads a file to OneDrive.
2. **Data Processing**:
   - The file is retrieved via **n8n** automation.
   - OpenAI Embedding 3 Small converts the file into vector data.
3. **AI Chatbot Processing**:
   - The vectorized data is passed to **ChatGPT 40 Mini**.
   - The AI agent responds with analysis, insights, or stock trends.
4. **User Interaction**: Users can query the agent for any analytical insights based on the uploaded file.

## n8n Workflow
The workflow in **n8n** consists of the following steps:
1. **Trigger**: Listens for new file uploads in OneDrive.
2. **File Retrieval**: Fetches the uploaded document.
3. **Preprocessing**: Converts the file into text format if necessary (e.g., extracting text from PDFs).
4. **Embedding Generation**: Uses OpenAI Embedding 3 Small to transform the text into vector representations.
5. **Chatbot Processing**: Sends the vectorized data to ChatGPT 40 Mini for generating analytical insights.
6. **Response Delivery**: Returns the generated insights to the user via n8n or a chat interface.

## Workflow Diagrams

### Data Upload (RAG Workflow)
![Screenshot 2025-03-23 131036](https://github.com/user-attachments/assets/5e67d7c3-d86a-49b3-8296-bcb4a540b606)


### Agent for Data Retrieval
![Screenshot 2025-03-23 131020](https://github.com/user-attachments/assets/be2d331f-8cbe-48f7-8a79-54753c40ef06)


## Installation & Setup
### Prerequisites
- **n8n** installed ([Installation Guide](https://docs.n8n.io/))
- **OneDrive API access** (linked to n8n)
- **OpenAI API Key** (for embedding and ChatGPT 40 Mini)

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/amityadav72/AI-Agent-as-Analyst.git
   cd AI-Agent-as-Analyst
   ```
2. Configure **n8n**:
   - Import the provided n8n workflow JSON.
   - Set up OneDrive integration for automatic file retrieval.
   - Add OpenAI API keys in the workflow settings.
3. Start **n8n**:
   ```sh
   n8n start
   ```
4. Upload a file to OneDrive and interact with the chatbot!

## Usage
- Upload a **CSV, Excel, PDF, or text file** containing stock data, financial records, or any analytical data.
- Ask questions like:
  ```
  - "What are the key trends in this stock data?"
  - "Analyze the sales performance over the last 3 months."
  - "Predict potential stock movements based on historical patterns."
  - "Summarize the key insights from this document."
  ```
- Get AI-driven insights powered by **ChatGPT 40 Mini**!

## Future Enhancements
- Integration with **Google Drive & Dropbox**.
- Real-time **stock market API** support.
- **Multi-user** support & web interface.
- **Advanced AI analytics** with visualization.
- **Support for more document formats (PPT, JSON, etc.)**.

## Contributing
Contributions are welcome! Feel free to submit issues, feature requests, or pull requests.

## License
This project is licensed under the MIT License.

---
### ✨ Connect with Me
📧 **Email**: [988981amityadav@gmail.com](mailto:988981amityadav@gmail.com)  
🔗 **LinkedIn**: [Amit Kumar Yadav](https://www.linkedin.com/in/amityadav72)  

---
🚀 Built with ❤️ using n8n, OpenAI, and OneDrive
