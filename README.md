# 🧠 Drug Discovery Agent with AI Reasoning (Cloud Deployed)

## 🔗 Live Demo (Cloud)

**Render Deployment URL:** [https://durg-discovery-agent-with-mcp-integration-fokr.onrender.com](https://durg-discovery-agent-with-mcp-integration-fokr.onrender.com)

👉 To interact with the project, open:

https://durg-discovery-agent-with-mcp-integration-fokr.onrender.com/docs

## 📌 Project Overview

This project is an **AI-powered Drug Discovery Agent** designed to assist in early-stage research by:

* Understanding biomedical and drug discovery–related queries
* Generating AI-driven insights using Large Language Models (LLMs)
* Performing reasoning and **fact-checking** on generated responses
* Providing structured **recommendations and explanations**

The system is built as a **backend API** using FastAPI and LangChain, and is fully **deployed on the cloud** so that anyone can access and test it.

This project demonstrates not only AI/GenAI development skills, but also **real-world cloud deployment, API design, and production readiness**.

---

## 🚀 What’s New (Compared to Local Version)

* ✅ Deployed the Drug Discovery Agent on **Render Cloud**
* ✅ Publicly accessible API endpoint
* ✅ Interactive **Swagger UI** for testing
* ✅ Environment-based configuration for secure API keys
* ✅ **Server URL and port updated to match Render’s default server startup requirements**

---

## 🛠️ Tech Stack

* **Language:** Python
* **API Framework:** FastAPI
* **Agent Framework:** LangChain
* **LLM Provider:** Groq LLM
* **Server:** Uvicorn
* **Cloud Platform:** Render (Free Tier)
* **API Testing Tool:** Swagger UI

---

## 🏗️ Project Architecture

project-root/
│── api_server.py              # FastAPI application entry point
│── agent/
│   ├── main_agent.py          # Core agent logic
│   ├── prompts.py             # Prompt templates
│── requirements.txt           # Project dependencies
│── README.md                  # Documentation


## ☁️ Cloud Deployment Details

### Why Render?

Render was chosen specifically to gain **real-world cloud deployment experience** using a 100% free platform.

**Advantages:**

* Free tier suitable for demo and portfolio projects
* No credit card required
* Simple GitHub-based CI/CD
* Automatic builds and deployments
* Ideal for FastAPI + Uvicorn applications

**Limitations:**

* Cold start delay on free tier
* Limited CPU and memory
* Not suitable for high-traffic production workloads

---

### 🔧 Important Deployment Configuration Change

To make the application compatible with **Render’s default web service environment**, the server configuration was updated:

* The FastAPI app binds to **`0.0.0.0`** instead of `localhost`
* The port is dynamically read from Render’s environment (default **port 10000**)
* The server start command aligns with Render’s default service behavior

This change ensures the application starts correctly on Render and that the platform can automatically detect the open port.

---

## ▶️ How to Use the Project (Step-by-Step)

### Step 1: Open the Live Cloud Link

Visit the deployed API:

https://durg-discovery-agent-with-mcp-integration-fokr.onrender.com

You should see a basic response confirming the server is running.

### Step 2: Open Swagger API Documentation

Append /docs to the URL:

https://durg-discovery-agent-with-mcp-integration-fokr.onrender.com/docs

This opens **Swagger UI**, an interactive API playground.

---

### Step 3: Select the POST Endpoint

* Locate the available **POST** endpoint
* Click on it to expand the details

---

### Step 4: Click “Try it out”

* Click the **Try it out** button
* Edit the request body
* Enter your query

Example:

json
{
  "query": "Suggest potential drug targets for breast cancer"
}

---

### Step 5: Execute the Request

* Click **Execute**
* Wait for the API response (first request may take longer due to cold start)

---

### Step 6: View the Results

The response includes:

* ✅ AI-generated answer
* ✅ Fact-checking output
* ✅ Reasoning and recommendations

---

## 🧪 Example Use Cases

* AI-assisted drug discovery research
* Biomedical question answering
* Educational and research tools
* GenAI backend services
* Demonstration of agent-based LLM systems

---

## ⚠️ Challenges Faced & Learnings

* Dependency conflicts between LangChain modules
* Aligning LLM-related package versions
* Port binding issues during cloud deployment
* Understanding cloud platform startup behavior

✔️ These were resolved by version alignment, environment-based configuration, and adapting the server startup to cloud requirements.

---

## 📈 Future Enhancements

* Add a frontend UI (Streamlit / React)
* Chat-based interaction instead of single queries
* Authentication and rate limiting
* Logging and monitoring
* Support for multiple LLM providers

---

## 👩‍💻 Author

M. SaiSushma 
B.Tech CSE (AI & ML) Graduate
Aspiring AI / GenAI Engineer

---

## ⭐ Support

If you find this project useful or interesting, please consider giving it a **star ⭐** on GitHub.
