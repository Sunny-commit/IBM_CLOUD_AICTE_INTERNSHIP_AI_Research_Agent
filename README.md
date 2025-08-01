# IBM_CLOUD_AI_Research_Agent

# 🤖 IBM Cloud watsonx.ai Agent Interaction Script

This repository contains a Python script designed to interact with an AI agent deployed on IBM Cloud's watsonx.ai platform. It provides a simple command-line interface for sending messages to your deployed AI model and receiving streaming responses, complete with conversation history for contextual interactions.

## ✨ Features

* **Real-time Interaction:** Send messages to your watsonx.ai deployed AI agent and receive responses.
* **Streaming Output:** Handles streaming responses from the `ai_service_stream` endpoint for a more dynamic chat experience.
* **Conversation History:** Maintains and sends conversation history to the AI agent, enabling multi-turn, contextual dialogues.
* **Secure API Key Handling:** Prompts for the API key at runtime, preventing hardcoding (though for production, environment variables or secret management are recommended).

## 🚀 Getting Started

Follow these steps to set up and run the script locally.

### Prerequisites

* Python 3.8+ installed on your system.
* An IBM Cloud account with a watsonx.ai service instance and a deployed AI agent.
* The `requests` Python library.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Sunny-commit/IBM_CLOUD_AI_Research_Agent]
.git)
    cd your-repo-name
    ```
2.  **Install dependencies:**
    ```bash
    pip install requests
    ```

### Configuration

1.  **Obtain your IBM Cloud API Key:**
    * Log in to your [IBM Cloud account](https://cloud.ibm.com/).
    * Navigate to `Manage` > `Access (IAM)`.
    * Click on `API keys` in the left navigation.
    * Click `Create an IBM Cloud API key` and copy the key.

2.  **Update the Deployment URL:**
    The script contains a placeholder `deployment_url`. You **must** replace this with the actual URL of your deployed AI agent on watsonx.ai.
    * Go to your watsonx.ai Studio on IBM Cloud.
    * Navigate to your `Deployment Spaces`.
    * Open the specific `Deployment Space` where your AI agent is deployed.
    * Go to the `Deployments` tab.
    * Click on the name of your deployed AI agent.
    * Look for the `API Reference` or `Endpoint` section to find your exact deployment URL. It should end with `/ai_service_stream`.

    Locate this line in the `main.py` (or your Python script file):
    ```python
    deployment_url = '[https://us-south.ml.cloud.ibm.com/ml/v4/deployments/d775e98a-77c0-4876-9b2b-76266ff7b91d/ai_service_stream?version=2021-05-01](https://us-south.ml.cloud.ibm.com/ml/v4/deployments/d775e98a-77c0-4876-9b2b-76266ff7b91d/ai_service_stream?version=2021-05-01)'
    ```
    And replace `d775e98a-77c0-4876-9b2b-76266ff7b91d` and potentially the region (`us-south`) with your specific details.

### Usage

Run the script from your terminal:

```bash
python AI_Research_Agent.py
