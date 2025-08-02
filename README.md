# IBM_CLOUD_AI_Research_Agent

## 🤖 IBM Cloud watsonx.ai Agent Interaction Script

This repository contains a Python script designed to interact with an AI agent deployed on IBM Cloud's watsonx.ai platform. It provides a simple command-line interface for sending messages to your deployed AI model and receiving streaming responses, complete with conversation history for contextual interactions.

---

## ✨ Features

- **Real-time Interaction:** Communicate directly with your watsonx.ai-deployed AI agent.
- **Streaming Output:** Displays responses in real-time using the `ai_service_stream` endpoint.
- **Conversation History:** Maintains multi-turn context for more natural interactions.
- **Secure API Key Handling:** Prompts for the API key at runtime (can be improved with environment variables for production use).

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- IBM Cloud account with watsonx.ai instance and deployed agent
- `requests` Python library

### Installation

1. **Clone the repository:**

    ```bash
    https://github.com/Sunny-commit/IBM_CLOUD_AICTE_INTERNSHIP_AI_Research_Agent.git
    cd IBM_CLOUD_AI_Research_Agent
    ```

2. **Install dependencies:**

    ```bash
    pip install requests
    ```

---

## ⚙️ Configuration

### 1. Obtain Your IBM Cloud API Key:

- Log into your [IBM Cloud account](https://cloud.ibm.com/)
- Go to **Manage > Access (IAM) > API keys**
- Create and copy a new API key

### 2. Update the Deployment URL:

Replace the `deployment_url` placeholder in your Python script with your actual deployment URL from the watsonx.ai deployment page.

```python
deployment_url = 'https://us-south.ml.cloud.ibm.com/ml/v4/deployments/YOUR_DEPLOYMENT_ID/ai_service_stream?version=2021-05-01'
```

Update the region and deployment ID accordingly.

---

## 💻 Usage

Run the script:

```bash
python AI_Research_Agent.py
```

You’ll be prompted to enter your IBM Cloud API Key. Once authenticated, you can chat with your AI agent.

Use `exit` or `quit` to end the session.

---

## 📸 Screenshots

### 🖼 Screenshot 1: Research AI Agent Normal Frontend View 
![Running the script](https://github.com/Sunny-commit/IBM_CLOUD_AICTE_INTERNSHIP_AI_Research_Agent/blob/main/images/AI%20Research%20Agent%20%E2%80%94%20ai_research_agent%20_%20IBM%20watsonx_00.png)

---

### 🖼 Screenshot 2: Research AI Agent Giving Information About How is artificial intelligence transforming healthcare diagnostics?
![Conversation in progress](https://github.com/Sunny-commit/IBM_CLOUD_AICTE_INTERNSHIP_AI_Research_Agent/blob/main/images/AI%20Research%20Agent%20%E2%80%94%20ai_research_agent%20_%20IBM%20watsonx_2_00.png)

---

### 🖼 Screenshot 3: Research AI Agent Giving Information About What are the benefits and challenges of hybrid education models? 
![Full response with history](https://github.com/Sunny-commit/IBM_CLOUD_AICTE_INTERNSHIP_AI_Research_Agent/blob/main/images/AI%20Research%20Agent%20%E2%80%94%20ai_research_agent%20_%20IBM%20watsonx_3_00.png)

---

## ⚠️ IBM Cloud Lite Plan Considerations

If using the Lite plan:

- You're limited to one watsonx.ai project or service instance.
- Export assets before deleting a project to create a new one.
- This client script should always be version-controlled on GitHub to avoid losing local files.

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request with improvements or bug fixes.

---


