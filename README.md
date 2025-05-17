# 🚀 Zero YAML, One Click: How I Used AI to Automate CI/CD on Kubernetes

> ✨ *"From a natural language prompt to a deployed, tested, validated Kubernetes application — all without writing a single YAML file."*  
> **Built with AI, Docker, Kubernetes, and ❤️**

---

## 🧠 What Is This?

**Zero YAML CI/CD** is a versioned, fully Dockerized system that brings the magic of AI to Kubernetes.  
It enables developers, DevOps engineers, and learners to build, deploy, test, and monitor applications using **natural language prompts** — without touching a single line of YAML.

Each version of the project adds a new layer of functionality, like a chapter in a technical storybook, building up to a complete **AI-powered CI/CD copilot experience**.

---

## 🌈 The Journey: Versioned Roadmap

Each version is a branch in this repository — designed to be used live in workshops, demos, and real-world learning.

| Version | Description                                                                                 | Highlights                                                 |
|---------|---------------------------------------------------------------------------------------------|------------------------------------------------------------|
| ✅ `v1-chat-ui-basic` | Chat UI + OpenAI-based YAML generation + K8s deployment + Testcontainers validation | Your prompt = deployed app, no YAML involved               |
| 🔄 `v2-validation-autoheal` | Smart error correction, re-prompts AI, rollback support                         | Self-healing CI/CD pipelines                               |
| 📊 `v3-observability` | Add Prometheus + Grafana dashboards                                                | Real-time metrics and health visibility                    |

> 🔜 V4 and V5 coming soon in future README updates

---

## 🐳 Why It’s Special

- 🔥 **AI-powered**: Uses GPT/OpenAI and later local LLMs (Mistral, Ollama, etc.)
- 🧠 **Zero YAML**: You never write YAML — it’s generated, validated, and tested automatically
- 🧪 **Built-in Testing**: Uses Python Testcontainers to validate live deployments
- 📦 **100% Dockerized**: No local installs; runs via `docker-compose up --build`
- 🌐 **Interactive UI**: Chat-based interface with live feedback and logs
- 🎯 **Workshop-Ready**: Designed for conferences, education, and hands-on learning

---

## 🧭 Repository Structure

```bash
zero-yaml-ci-cd/
├── backend/             # FastAPI backend (GPT → YAML → K8s apply → Testcontainers)
├── frontend/            # Chat UI (React or HTML/JS)
├── shared/              # Prompt templates, utilities (optional)
├── docker-compose.yml   # Runs everything: frontend, backend, kind cluster
├── .env.example         # Env for OpenAI key or local SLM
└── README.md            # This file (main branch)
```

---

## ⚙️ Tech Stack

| Area           | Tools & Technologies                                 |
|----------------|------------------------------------------------------|
| Frontend       | Vanilla JS or React (chat UI)                        |
| Backend        | FastAPI (Python)                                     |
| AI Engine      | GPT-4 (OpenAI API) → later: Local SLMs (Ollama, LM Studio) |
| Kubernetes     | kind (Kubernetes in Docker)                          |
| Validation     | Testcontainers (Python)                              |
| Infra Control  | `kubectl`, Python Kubernetes SDK                     |
| Monitoring     | Prometheus + Grafana (V3)                            |

---

## 🧪 Testcontainers: Our Secret Superpower

Unlike most demos, **we don’t just deploy — we validate**.  
After YAMLs are applied, Testcontainers runs automated integration tests like:

- ✅ Ping NGINX and FastAPI endpoints
- ✅ Connect to MongoDB
- ✅ Confirm services are healthy

Every version uses Testcontainers to ensure reliability.

---

## 🔐 Security & Best Practices

- 🔒 OpenAI key managed through `.env`, not hardcoded
- 🔒 YAMLs are validated before applied
- 🔒 All subprocess calls are safe and logged
- 🧱 Built to be scalable and MVP-ready

---

## 🧱 Contributing

Want to improve this? Add new prompts? Support more LLMs?

1. Fork this repo
2. Pick a version branch (e.g., `v1-chat-ui-basic`)
3. Submit a pull request with a clear message

---

## 👨‍🏫 Who Is This For?

- 🔧 Developers tired of boilerplate YAML
- 🎓 Students learning DevOps/Kubernetes
- 🧪 Engineers building CI/CD pipelines
- 📢 Speakers and educators doing live demos

---

## 🧠 Inspiration

> This project follows **Steve Jobs' "connecting the dots" philosophy** — every version unveils something new, exciting, and meaningful. It's built not just to impress, but to educate and inspire.

---

## 📸 Screenshots (Add per version)

> ✅ Coming soon: screenshots of chat UI, live deployments, logs, diagrams...

---

## 📣 Follow the Versions

You can switch versions via:

```bash
git checkout v1-chat-ui-basic  # or v2-validation-autoheal, etc.
```

Run with:

```bash
docker-compose up --build
```

---

## ❤️ Built by [@vellankikoti](https://github.com/vellankikoti)

Follow, fork, and create unforgettable DevOps + AI experiences.

> _“DevOps shouldn’t feel like plumbing. It should feel like magic.”_
