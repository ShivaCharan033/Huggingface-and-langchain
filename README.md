# 🧠 Running LLMs Locally with LangChain + Hugging Face

This project demonstrates how to run **Large Language Models (LLMs)** locally using **LangChain** in combination with the **Hugging Face Hub**, directly from environments like **Google Colab**. The aim is to showcase how open-weight models like Mistral, LLaMA, and Falcon can be invoked and tested for prompt-based generation using LangChain’s integration capabilities.

---

## 📌 Project Objective

To explore and test how open-source LLMs can be run **locally** or via **Hugging Face Inference Endpoints** using the `langchain-huggingface` wrapper. The project also demonstrates best practices in authentication, prompt structuring, and runtime behavior of popular instruction-tuned models.

---

## 🚀 What I Did

### 🔐 Token Authentication
- Stored Hugging Face access token securely using `google.colab.userdata` in Colab.
- Passed the token to LangChain and Hugging Face APIs using Python’s `os.environ`.

### 🔗 Model Integration
- Used the `HuggingFaceEndpoint` wrapper from `langchain_huggingface` to connect to models hosted on the Hugging Face Hub.
- Integrated models like:
  - `mistralai/Mistral-7B-Instruct-v0.3`
  - `meta-llama/Llama-2-7b-chat-hf`
  - `tiiuae/falcon-7b-instruct`

### ⚙️ LangChain Usage
- Configured the LLMs with key parameters like `max_length` and `temperature`.
- Called `.invoke()` to send prompts and receive model completions.

### 🧪 Prompt Testing
- Sent multiple prompts to evaluate model responses.
- Adjusted parameters to control verbosity and creativity of the output.

### 💻 Google Colab Setup
- Installed required libraries: `langchain-huggingface`, `huggingface_hub`, `transformers`, `accelerate`, `bitsandbytes`.
- Verified GPU compatibility to support faster execution of model queries.

### 🧵 Toolchain Integration
- Used `transformers` for backend operations and model control.
- Integrated `bitsandbytes` and `accelerate` to enable efficient memory usage for larger models.
- Cached models locally inside Colab environment to improve speed.

---

## 🔧 Technologies Used

- **LangChain**
- **Hugging Face Hub**
- **Transformers**
- **Accelerate**
- **Bitsandbytes**
- **Google Colab**
- **Python**

---

## 🧪 Models Explored

- `mistralai/Mistral-7B-Instruct-v0.3`
- `meta-llama/Llama-2-7b-chat-hf`
- `tiiuae/falcon-7b-instruct`

> You can replace these with any Hugging Face model that supports `text-generation` and open weights.

---

## 📦 Installation (in Google Colab)

```bash
!pip install langchain-huggingface
!pip install huggingface_hub
!pip install transformers
!pip install accelerate
!pip install bitsandbytes

## ✅ Features

- ✅ End-to-end LLM setup using Hugging Face + LangChain  
- 🔐 Secure token handling via Colab `userdata`  
- ✍️ Prompt-based invocation and output formatting  
- ⚡ Real-time interaction with instruction-tuned open-source models  
- ☁️ Run-time experimentation in cloud environment (Google Colab)  

---

## 🤖 Future Improvements

- 🧩 Extend with LangChain tools like chains and agents  
- 🌐 Add streaming output via WebSocket or Gradio interface  
- 🖥️ Support for local inference using `transformers.pipeline()` and CPU/GPU fallback  
- 🧪 UI to test prompts dynamically  

---

## 📫 Contact

**Shiva Charan Pailla**  
📧 shivacharanpailla@gmail.com  
 

---

## 🔐 Token Safety Note

> Please note: I have not included screenshots or runtime proofs in this public repository to avoid exposing sensitive Hugging Face tokens, which could be misused by others.  
> For any verification, I’m happy to demo the functionality securely upon request.

---

## 🙌 Acknowledgements

Huge thanks to the amazing communities behind:

- 🤗 **Hugging Face** – for hosting accessible open-weight models  
- 🦜 **LangChain** – for simplifying prompt interaction and LLM orchestration  
- 🧪 **Google Colab** – for making quick prototyping with GPUs easy and accessible  

