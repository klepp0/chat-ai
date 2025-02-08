# Chat-AI 🧠💬

A self-hosted chatbot setup that allows you to run **any locally installed LLM** using [Ollama](https://ollama.com).

<div align="center">

![Dockerized](https://img.shields.io/badge/Dockerized-Yes-blue)
![Self-Hosted](https://img.shields.io/badge/Self--Hosted-Yes-green)
![Local LLMs](https://img.shields.io/badge/Local%20LLMs-Supported-purple)

</div>

## 🚀 Features

✅ **Run any local LLM** with Ollama  
✅ **Pre-configured Docker setup** for easy deployment  
✅ **Web-based chat UI** for interaction  
✅ **Easily install new models**

---

## 🛠️ Setup & Usage

### 🔥 Start the Chat-AI Service

To start all required services (**Ollama**, **Open WebUI**, and **MongoDB**), simply run:

```sh
docker compose up -d
```

This will spin up everything you need to start chatting locally in just a few seconds.

### 🤖 Install a New Model

Want to use a different model? No problem! Browse the [available models](https://ollama.com/search) and install any model directly into your Ollama service.

For example, to install [deepseek-r1](https://ollama.com/library/deepseek-r1), run:

```sh
docker exec -it chat-ai-ollama-service-1 ollama pull deepseek-r1
```

Once installed, you can use the model immediately.

### 💻 Access the Chat Interface

Once the services are running, open your favorite browser and head to:

🔗 [http://localhost:3000](http://localhost:3000)

This will load the Open WebUI, where you can chat with your locally hosted AI assistant.

### 🛑 Stop the Chat-AI Service

To gracefully stop all running containers, run:

```sh
docker compose down
```

This will shut everything down while keeping your data intact.

### 🛠️ How It Works

Chat-AI leverages the power of Ollama to run LLMs locally, MongoDB for conversation history, and Open WebUI as the front-end chat interface. The entire stack is wrapped neatly in Docker for easy deployment.

### 💡 Why Use Chat-AI?

🚀 No API limits – You control your own AI assistant
🛡 Privacy-first – Your chats stay on your machine
⚡ Flexibility – Use any LLM that Ollama supports
🔧 Extensible – Customize and integrate as needed

Happy chatting! 💬🤖✨
