<div align="center">

# Bhavdeep Singh

**Final-year B.Tech @ IIT Roorkee**

AI Engineering · Full-Stack Development · LLM Systems

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bhavdeep-singh-107b36252/)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:singhbhavdeep364@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/Bhavd33p)

</div>

---

## About

I build AI systems that ship — from fine-tuning LLMs on custom hardware to full-stack apps with real auth and real users. I care about making things fast, reliable, and cost-efficient. Currently looking to join an early-stage team as a Software / AI Engineer where I can own features end-to-end.

---

## Projects

### 🧠 Multi-Tenant LLM Serving Engine
> *Production inference server — multiple LoRA adapters, one quantized base model*

FastAPI server that hot-swaps between task-specific LoRA adapters (code generation, finance extraction) on a 4-bit quantized Qwen2.5 model. Trained adapters from scratch on Apple Silicon using custom data pipelines.

- **4-bit NF4 quantization** — ~75% memory reduction, fits on consumer GPU/MPS
- **O(1) adapter switching** — pointer swap at inference time, no reload overhead
- **Streaming SSE responses** — token-by-token via `TextIteratorStreamer` + async FastAPI
- **Full training pipeline** — data prep → LoRA fine-tuning → adapter serving in one repo

`FastAPI` `PyTorch` `HuggingFace` `LoRA/PEFT` `BitsAndBytes` `Apple Silicon MPS`

[→ View Repo](https://github.com/Bhavd33p/multi-tenant-llm-engine)

---

### 🤖 AI TestCase Generator
> *RAG pipeline that turns requirement docs into test cases*

Ingests SWAD/ICD/BRD documents and generates structured test cases using adaptive retrieval and feedback loops. Benchmarked on RTX 4090.

- Adaptive RAG with vector search over requirement chunks
- Human-in-the-loop feedback for iterative refinement
- Cuts manual test case writing by ~70–80%

`Python` `LangChain` `RAG` `Vector DBs` `FastAPI`

[→ View Repo](https://github.com/Bhavd33p/TestCase_Generator)

---

### 💬 PDF Converse
> *Multi-user collaborative chat over any PDF*

Upload a PDF, ask questions, get grounded answers. Multiple users, multiple threads, all indexed and retrieved with semantic search.

- Chunking + embeddings + conversational retrieval chain
- Multi-user session management with isolated threads
- Answers grounded strictly in uploaded document context

`Python` `LangChain` `Vector Embeddings` `FastAPI` `React`

[→ View Repo](https://github.com/Bhavd33p/PDF-Converse)

---

### ✅ Mini Task Manager
> *Full-stack project management with role-based auth*

End-to-end task and project management system. Clean API, JWT auth, role separation, due dates.

- .NET backend + React + TypeScript frontend
- JWT authentication with role-based access control
- User-scoped projects and tasks with due date tracking

`.NET` `React` `TypeScript` `JWT` `PostgreSQL`

[→ View Repo](https://github.com/Bhavd33p/Mini-Task-Manager)

---

### 🖊️ Web Annotator
> *Browser extension for in-place web annotation*

Chrome extension to highlight, underline, and annotate text on any webpage — saved persistently per-URL.

`JavaScript` `Chrome Extensions API` `DOM Manipulation`

[→ View Repo](https://github.com/Bhavd33p/Web-Annotator)

---

## Skills

**Languages**

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-%2307405E.svg?style=for-the-badge&logo=postgresql&logoColor=white)

**AI / ML**

![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/Hugging_Face-%23FFD21E.svg?style=for-the-badge&logo=huggingface&logoColor=white)
![LangChain](https://img.shields.io/badge/langchain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

**Backend / APIs**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)

**Frontend**

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Next.js](https://img.shields.io/badge/next.js-%23000000.svg?style=for-the-badge&logo=nextdotjs&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/postgresql-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)

**DevOps / Tools**

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)

---

## What I'm Looking For

Open to **Software Engineer** or **AI Engineer** roles at early-stage companies where I can:
- Own features from problem definition through design to production
- Build reliable, cost-efficient LLM systems and internal tooling
- Work on teams that move fast and care about quality

📬 **singhbhavdeep364@gmail.com** · [LinkedIn](https://www.linkedin.com/in/bhavdeep-singh-107b36252/)
