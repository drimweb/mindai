---
icon: diagram-venn
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# MindAI Orchestrator

## The Intelligence Engine Behind Autonomous Agents

The **MindAI Orchestrator** is a low code intelligence engine that governs agent behavior—empowering agents to think, plan, and act autonomously. It combines powerful foundation models, contextual reasoning, and a modular execution architecture to enable agents to operate intelligently within complex environments.

At its core, the Orchestrator translates **goals, personality, and real-time inputs** into **coordinated sequences of actions**, allowing agents to adapt, collaborate, and execute tasks across both Web3 and traditional systems.

### Modular, Context-Aware Autonomy

The Orchestrator is structured around a **hierarchical planning architecture**:

* **High-Level Planner**: Aligns long-term objectives, contextual signals, and personality traits with the agent’s intent.
* **Low-Code Executors**: Select and trigger modular tools, APIs, smart contract actions, or data-fetching workflows via the integrated [Morpheus Labs Workflow Studio](https://wfstudio.morpheuslabs.io).

This structure ensures that agents aren't just reactive—they’re strategic, goal-aligned, and capable of long-horizon planning.

### Deployment Options

The MindAI Orchestrator can be used in two complementary modes:

#### 🔹 **Cloud-Hosted Model** (Workflow Studio + Google Cloud)

A fully managed, low-code solution for orchestrating agent logic, tool usage, and AI reasoning. Ideal for creators, teams, and enterprise users who want to deploy intelligent agents without managing infrastructure.

**Features:**

* Agentic templates are visual workflows with trigger/action nodes
* Native support for onchain integrations, APIs, and AI models
* Auto-scaling via Cloud Run & Cloud Functions
* Agent memory stored in Firestore , Vertex AI Vector Search , BigQuery
* Secure model access through Vertex AI or containerized endpoints

**Includes prebuilt functions for Agents to do:**

* Webhooks, API calls, data enrichment
* Smart contract interactions (read/write)
* Agent-to-agent task coordination
* Token-actions (stake, vote, claim, mint)

***

#### 🔸 **Developer SDK Model**

For developers who want full control, the **MindAI Orchestrator SDK** provides a programmatic interface to embed orchestration logic into custom environments or run agents independently.

**Features:**

* Lightweight SDK to embed orchestration engine
* Supports integration with third-party LLMs and hosted models
* Plug-and-play compatibility with MindAI Exchange Protocol
* Local execution, or deployment via any preferred cloud
* Web3 plugin support (for Ethereum, Kusama, Solana, etc.)

**Supports:**

* Agent-to-agent commerce via MXP-compatible plugins
* Custom toolchains and evaluator modules
* Agent memory frameworks (in-memory, IPFS, Firestore, Postgres)
* Contribution of community plugins (image processing, governance, etc.)

***

### Hosted Foundation Models

MindAI supports and integrates with the following foundation models, hosted through Google Cloud (Vertex AI) or containerized on GKE:

* **Gemini / PaLM 2** (Google Cloud)
* **LLaMA 3 8B / 70B Instruct** (custom-hosted)
* **DeepSeek R1 & V3**
* **Qwen 2.5 72B Instruct**
* **OpenRouter-compatible models** (optional via SDK)

Agents can call models directly or compose reasoning steps using **prompt chains**, enabling both single-shot and multi-turn intelligence workflows.

