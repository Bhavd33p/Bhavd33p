<div align="center">

# Hi, I'm Bhavdeep 👋

🛠️ **Software Engineer @ Newton School** | 🎓 **IIT Roorkee '26** | 📍 **India**

**Infrastructure · Platform · Application Security**

</div>

![Go](https://img.shields.io/badge/-Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/-C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Django](https://img.shields.io/badge/-Django-092E20?style=flat-square&logo=django&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Prometheus](https://img.shields.io/badge/-Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)

> Software engineer working across backend, infrastructure and the systems layer in between —
> Go, Python and TypeScript in production. Most of what I find interesting sits below the
> feature: how things fail, where the boundaries are, and what holds up under load.
> Contributor to **Kubeflow** (CNCF ecosystem).

---

## Open Source — Kubeflow

**[kubeflow/kale](https://github.com/kubeflow/kale)** — notebook-to-pipeline toolchain

| PR | State | What |
|---|---|---|
| [#866](https://github.com/kubeflow/kale/pull/866) | ✅ **merged** | Configurable production PyPI index via `KALE_PYPI_PROD_URL`, removing a hardcoded endpoint from the release path |
| [#842](https://github.com/kubeflow/kale/pull/842) | ✅ **merged** | Collapsed two deploy-progress abstractions into one |
| [#865](https://github.com/kubeflow/kale/pull/865) | 🔄 open | CLI support compiling notebooks into native Kubernetes manifests |
| [#935](https://github.com/kubeflow/kale/pull/935) | 🔄 open | Removed enum drift between Python and TypeScript definitions by deriving both from one JSON source |
| [#934](https://github.com/kubeflow/kale/pull/934) | 🔄 open | Block invalid pipeline step names at input instead of warning after they reach metadata |
| [#906](https://github.com/kubeflow/kale/pull/906) | 🔄 open | Clear error when the pipeline backend is unreachable |

**[kubeflow/notebooks](https://github.com/kubeflow/notebooks)** — ML workspace platform

| PR | State | What |
|---|---|---|
| [#1204](https://github.com/kubeflow/notebooks/pull/1204) | 🔄 open | Workspace auto-pause countdown — culling-deadline computation against the `WorkspaceKind` CRD `cullingConfig` contract, with a 9-case unit suite |

---

## Building Now

🎛️ **Model Serving Platform on Kubernetes**
A `kubebuilder` operator managing the serving lifecycle of ML models through a custom
`InferenceService` CRD — reconcile loop, finalizers, owner references, status subresources.
Artifact pulls from S3-compatible storage with readiness gated on model-load completion,
canary rollout with traffic splitting, autoscaling on inference queue depth rather than CPU.

`Go` · `kubebuilder` · `controller-runtime` · `Kubernetes` · `Prometheus` · `MinIO`

📡 **Reliable UDP Transport Protocol**
A connection-oriented transport over UDP: state machine, selective-repeat ARQ with SACK,
sliding-window flow control, Jacobson/Karels RTT estimation with adaptive RTO. Pluggable
congestion control behind one interface, and per-stream configurable reliability — reliable,
unreliable, or deadline-bounded — so latency-sensitive traffic bypasses the head-of-line
blocking TCP enforces. Benchmarked against TCP and raw UDP under `tc netem`.

`C++` · `UDP` · `tc/netem` · `Prometheus` · `GitHub Actions`

---

## Shipped

⏱️ **TimeTracker** — 🔴 **[live at timetracker-day.vercel.app](https://timetracker-day.vercel.app/)**
Plan a day in time blocks, keep tasks beside them, and see where the week actually went.
An installable PWA that works fully offline and syncs to Firestore on sign-in. The service
worker is **network-first over content-hashed assets** — so a new deploy reaches an already
installed app on its next online open, with no precache manifest to keep in step.

`React` · `Vite` · `Firebase / Firestore` · `PWA` · `service worker` · `Vercel`

🏦 **[FinTech Multi-Agent System](https://github.com/Bhavd33p/FinTech-Multi-Agent-System-)**
Five specialist agents — financial analysis, risk scoring, portfolio allocation, fraud detection,
regulatory compliance — behind an orchestrator doing intent classification and running them
standalone, sequentially or in parallel. Wrapped in real guardrails: **prompt-injection detection**
across 15+ pattern rules, PII redaction and disallowed-topic blocking on input; disclaimer
injection, hallucination detection and length bounding on output. Compliance covers RBI, SEBI,
PMLA, FEMA and the DPDP Act.

`Python` · `Claude SDK` · `tool use` · `guardrails`

⚡ **Multi-Adapter LLM Serving Infrastructure**
Single-process inference server hosting two LoRA adapters on a shared Qwen-2.5 base with
header-based routing and runtime hot-swapping, removing the cost of one GPU deployment per
model. 4-bit NF4 quantization cut memory footprint **68%**, sustaining 15–30 tok/s at
**sub-500ms** time-to-first-token, with token-level streaming.

`Python` · `FastAPI` · `PyTorch` · `QLoRA` · `Transformers`

📋 **[Mini Task Manager](https://github.com/Bhavd33p/Mini-Task-Manager)**
Full-stack project management system — .NET backend, React + TypeScript frontend, JWT auth and
user-scoped projects. Containerized end to end with separate backend and frontend images,
docker-compose orchestration and an nginx reverse proxy.

`C#` · `.NET` · `React` · `TypeScript` · `Docker` · `nginx`

🚕 **[Pink Taxi](https://github.com/Bhavd33p/pink-taxi)**
Ride-hailing app built around women's safety in India — Flutter client, Firebase backend,
Cloud Functions.

`Flutter` · `Dart` · `Firebase`

📄 **[PDF Converse](https://github.com/Bhavd33p/PDF-Converse)** · ✍️ **[Web Annotator](https://github.com/Bhavd33p/Web-Annotator)**
Retrieval-based question answering over uploaded PDFs; and a browser extension for highlighting,
underlining and annotating text on any web page.

`Python` · `JavaScript`

---

## Experience

**Newton School** — Software Engineer · *June 2026 – present*
Backend and platform work across Python/Django, Go and TypeScript — sandboxed execution of
untrusted code, distributed task correctness, API performance, and application security.

**Zinnia Digital Services** — Software Engineering Intern · *May – July 2025*
Document ingestion and embedding pipelines over ChromaDB, and REST APIs for inference and
validation.

---

## Connect

[![Email](https://img.shields.io/badge/-Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:singhbhavdeep364@gmail.com)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bhavdeep-singh-107b36252/)
[![LeetCode](https://img.shields.io/badge/-LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=white)](https://leetcode.com/u/wMPj0n1bvp/)
[![GitHub](https://img.shields.io/badge/-Follow-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Bhavd33p)

**IIT Roorkee**, B.Tech 2026 · LeetCode peak **1853** · CodeChef peak **1647** (`Sirius3`) · 1000+ problems solved
