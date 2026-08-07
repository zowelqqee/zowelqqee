# Hi, I'm Arseniy 👋

**ML Engineer / AI Developer**

I build machine learning systems end-to-end — from experiments and model training to inference APIs, CI/CD, and production deployment.

My current work focuses on **AI systems, reasoning architectures, knowledge graphs, and reliable ML**: systems where decisions can be inspected, reproduced, and evaluated rather than treated as opaque model outputs.

Currently studying **Applied Mathematics and Computer Science** at Peter the Great St. Petersburg Polytechnic University.

---

## 🧩 MicroWorld

**An explicit semantic runtime for deterministic and auditable AI.**

MicroWorld explores an AI architecture where semantic memory, reasoning, dialogue state, and language generation are separate, inspectable runtime components.

The core reasoning path does not depend on a trainable neural model.

**Results:**
- 100% accuracy on held-out compositional reasoning and paraphrased queries in the current benchmark
- Qwen2.5 0.5B–7B baselines: 60–90% on the same evaluation
- 100% correct abstention across evaluated test sets
- ~8 ms p50 latency on Apple M1 CPU
- Fully local execution
- Deployed offline on an iPhone 11

`Python` `FastAPI` `spaCy` `Knowledge Graphs` `Symbolic Reasoning`

---

## 🛡️ Fraud Detection & AML

I am currently testing whether the same explicit semantic architecture can transfer to real ML domains.

### AML

Hybrid raw + semantic features improved fraud detection by:

- **+1.18 pp recall**
- **338 fewer false positives**

### IEEE-CIS Card Fraud

Transferred the same architecture to a 590K-row card fraud dataset:

- **+3.1 pp recall**
- **126 additional fraud cases detected**

I also document negative results and trade-offs — including cases where higher recall comes with more false positives at a fixed threshold.

`Python` `Machine Learning` `Graph Reasoning` `Fraud Detection` `AML`

---

## 🤖 JARVIS

Local AI agent for computer interaction and task execution.

- Intent classification with TF-IDF + Logistic Regression
- **97.6% accuracy** on ~4K examples
- 15+ tracked MLflow experiments
- FastAPI backend
- PySide6 desktop application
- Browser and system-level automation

`Python` `scikit-learn` `FastAPI` `MLflow` `PySide6`

---

## 🌍 SafeLanding

B2B2C relocation platform with an end-to-end ML pipeline.

Built a multi-head PyTorch model for:

- city ranking
- risk prediction
- explanation generation

Trained across data for **81 cities**, with MLflow experiment tracking, FastAPI inference, continual learning from user interactions, and GitHub Actions CI/CD.

`PyTorch` `FastAPI` `MLflow` `Supabase` `Next.js`

---

## 🧠 micrograd

A tiny deep learning framework built from scratch in pure Python.

Implemented:

- scalar-valued autograd
- computation graphs
- reverse-mode backpropagation
- SGD
- multilayer perceptrons
- nonlinear classification training

No ML frameworks.

---

## 🔬 What I'm interested in

Machine Learning · Deep Learning · AI Systems · Reasoning Systems · Knowledge Graphs · Explainable AI · Information Retrieval · AI Infrastructure

---

## 🛠 Stack

**ML / AI**  
Python · PyTorch · scikit-learn · MLflow · OpenCV · spaCy · NLP · Computer Vision

**AI Systems**  
Knowledge Graphs · Symbolic Reasoning · RAG · LLM APIs · Vector Databases

**Backend / Infrastructure**  
FastAPI · PostgreSQL · Supabase · Docker · REST APIs · GitHub Actions · CI/CD

**Other**  
TypeScript · C++

---

## 📫 Contact

LinkedIn: arseniy-abramidze-14946727b  
Email: zowel.aep@gmail.com
