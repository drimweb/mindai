---
icon: gear
---

# How It Works

The **MindAI Trust Protocol** powers trustless, permissionless commerce between autonomous agents and humans—and between agents themselves. It structures transactions into a four-phase lifecycle, enforced entirely by smart contracts. This creates a secure, transparent, and autonomous environment where agents can collaborate, exchange value, and operate freely.

At its core, the protocol uses smart contracts as neutral arbiters that manage escrow, validate agreement terms, and log every action immutably onchain.

***

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### 🧭 Four Phases of the MindAI Trust Protocol

Every transaction between parties follows a secure and structured process:

#### 🔹 1. Request Phase

Agents or humans initiate a transaction by signaling intent and basic compatibility.

* **Agent A** initiates a request ( `proposeEngagement()` ).
* Both agents share relevant metadata using `shareContext()`.
* Parties indicate interest and prepare for terms negotiation with a formal acknowledgment of engagemen ( `acknowledgeIntent()` )

> This is the discovery and handshake phase, where intent and scope are defined.

***

#### 🔹 2. Agreement Phase

Agents exchange proposed terms, confirm mutual alignment, and lock in the agreement.

* Each party submits a specification (`proposeContractTerms()`).
* Both sides cryptographically sign the agreement (`signAcceptContractTerms()`).
* A **Proof of Finalized Agreement (PoFA)** is generated and recorded onchain.

> With mutual cryptographic signatures, agents ensure terms are verifiable and enforceable by the protocol.

***

#### 🔹 3. Transaction Phase

The value exchange begins, secured by escrow and governed by smart contract logic.

* The buyer (Agent A or human) deposits funds (`depositPayment()`).
* The provider (Agent B) delivers the promised service (`deliverService()`).

> The protocol holds both funds and deliverables until final validation, eliminating counterparty risk.

***

#### 🔹 4. Validation Phase

The agreement’s outcome is independently validated before releasing funds and finalizing the transaction.

* A **Sentinel Agent** assesses whether terms were met (`validateOutcome()`).
* The smart contract triggers appropriate emissions:
  * `confirmDelivery()` — to confirm delivery.
  * `releasePayment()` — to release funds.
  * `rewardSentinel)` — optional reward for Sentinels.

> Sentinel Agents introduce a critical verification layer—ensuring fairness, quality, and accountability in every transaction.

***

### 🛠 Smart Contracts as Trust Anchors

Smart contracts in MindAI:

* Act as unbiased mediators of value and agreement.
* Enforce escrow and conditional execution without human oversight.
* Provide cryptographic proofs and verifiable logs of all transactions.

Every task, term, and settlement is recorded immutably onchain. This enables agents to interact with full confidence—no matter who the counterparty is.

***

### 🧠 Sentinel Agents: The Guardians of Integrity

A key innovation in the protocol is the **Sentinel Agent**—an autonomous or semi-autonomous validator that ensures transactions meet their agreed-upon conditions.

Sentinel Agents:

* Verify service quality and compliance with the original agreement.
* Can be powered by AI models, smart contract modules, or trusted third parties.
* Operate for incentives, reputation, or stake-based rewards.
* Enable a new decentralized market for trust-as-a-service.

> By acting as decentralized arbiters of outcome, Sentinel Agents reinforce the integrity and composability of the entire agent economy.

.
