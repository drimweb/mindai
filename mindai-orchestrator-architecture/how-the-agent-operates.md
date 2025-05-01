# How the Agent Operates

How the Agent Operates (Perception → Reasoning → Action)

MindAI Agents are designed to behave autonomously by following a structured intelligence loop composed of three stages: **Perception**, **Reasoning**, and **Action**. This design allows agents to dynamically respond to inputs, make decisions using AI models, and execute verified outputs onchain using Web3 logic.

Based on the [MindAI Orchestrator Architecture](./) we derive that the Perception and Action are part of the External Inputs and Orchestration Core layers  while the Reasoning is part of the Model & Reasoning layer.&#x20;

In a simplified view, the orchestration of this behavior is achieved using **Workflow Studio**, a low-code environment that integrates with **AI** and Web2/Web3 action nodes.&#x20;

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption><p>A simplified diagram showing how the AI  Agent operates</p></figcaption></figure>

### 1. Perception

**Perception** is the agent’s ability to receive signals from the world. These can come from user requests, external events, smart contract data, or off-chain services.

In Workflow Studio, this is handled using:

* **Trigger Nodes** — monitor onchain and off chain events.
* **Webhook Nodes** — capture HTTP requests, form submissions, or API calls.

**Examples**:

* Detect a Twitter mention to activate a KOL agent.
* Receive a new DAO proposal submission via webhook.
* Monitor a wallet balance falling below a threshold.

***

### 2. Reasoning

**Reasoning** allows the agent to interpret context, apply logic, and decide on the next action. This layer is powered by **Google Cloud AI**, particularly:

* **Vertex AI LLMs** (e.g. PaLM, Gemini) for language understanding and strategic decision-making.
* **Imagen** for image generation (e.g. marketing content).
* **Speech-to-Text / Audio-to-Gesture** pipelines for multimodal input analysis.

The agent interprets intent and routes decisions to the appropriate output logic.

**Examples**:

* Classify if a user’s message should trigger a paid service.
* Generate custom visual content for a marketing campaign.
* Decide whether to accept or reject a smart contract proposal.

***

### 3. Action

**Action** is where agents interact with the external world—most often onchain. Using **Action Nodes** in Workflow Studio, agents can:

* Execute smart contract functions
* Transfer or stake tokens
* Mint NFTs or generate invoices
* Store files to IPFS or update databases

These actions are secure, auditable, and permissionless.

**Examples**:

* Transfer $MINDAI to a user after a successful evaluation.
* Mint a proof-of-contribution NFT.
* Execute a buy order on a decentralized exchange.

***

### Workflow Summary

```plaintext
[Trigger or Webhook]
       ↓
[Google Cloud Reasoning (LLM, Imagen, etc.)]
       ↓
[Action Node (e.g. mintNFT, transferToken, executeSmartContract)]
       ↓
[Onchain Result validation via MindAI Trust Protocol]
```
