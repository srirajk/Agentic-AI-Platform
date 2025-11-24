# Storyline – Thin Client + EY Assets + Templates + 7-Layer Platform

## 1. Purpose of This Storyline

This document gives us **one common storyline** we can all use when talking about our response to the AI platform RFP.

It is **not** a detailed architecture spec.  
It is a **narrative** we can use in:

- internal discussions,
- leadership prep,
- shaping slides and written RFP responses.

We can dial it **up or down** in detail depending on the audience.

---

## 2. The Core Message in One Paragraph

> The client doesn’t need just another bot or AI pilot.  
> They are asking for a **standard, governed way** to build and run AI agents on top of the cloud they already have.
>
> Our proposal is a **thin client layer** that sits on top of their existing environment, and we pack it with **EY assets** (like an agent test harness) and **templates** (for common use cases and governance patterns).
>
> Underneath that thin layer, the platform runs on a **cloud-native, model-agnostic runtime**, so they can evolve their model choices over time without redesigning everything.

This is the essence of our story.

---

## 3. Act 1 – Why a Platform, Not Just More Bots

**The problem we see:**

- There are many places where AI could help (documents, emails, exceptions, helpdesk, internal servicing flows).
- Different teams and vendors are experimenting with **one-off tools and pilots**.
- There is **no single, repeatable way** for the client to:
    - design agents,
    - test them properly,
    - run them in production with governance and cost control.

**What the RFP is really asking for:**

- A **no-code / low-code platform**, not another isolated chatbot.
- Something that technology leadership can **standardize on**:
    - multi-model capable,
    - secure and governed,
    - observable and cost-aware.

**Our framing for Act 1:**

> “The real challenge isn’t a lack of AI.  
> It’s the lack of a **platform** – a consistent, governed way for teams to build and run agents on top of the client’s existing cloud.”

---

## 4. Act 2 – Our Shape: Thin Client + EY Assets + Templates

### 4.1 Thin Client – Light Layer, Heavy Value

We are **not** dropping a big monolithic platform into their environment.

We propose a **thin client layer** that:

- Sits on top of their existing cloud and AI services.
- Provides a **single portal/experience** for:
    - discovering and configuring agents,
    - designing or tweaking workflows (no-code / low-code),
    - testing agents before promotion,
    - monitoring runs, exceptions, approvals.

**Key line:**

> “We bring a **thin client layer**, not a heavy new stack – a light experience and control surface on top of what the client already has.”

Where this maps conceptually:

- Experience for business users, developers, and admins.
- Top of the Builder space (no-code builder, configuration).
- Some aspects of Governance (approvals, visibility).

---

### 4.2 EY Assets – Especially the Agent Test Harness

The thin client isn’t empty.  
We embed **EY assets** that we already have and reuse:

- **Agent Validation & Test Harness**
    - Run agents against curated scenarios (emails, docs, workflows).
    - Compare expected vs actual outputs.
    - Works across different models/providers (model-agnostic).
    - Supports regression testing whenever something changes (prompts, flows, tools).

- **Governance Patterns**
    - Predefined role models (who can build / approve / run).
    - Human-in-the-loop patterns (when a human must review/approve).

- **Integration & Workflow Patterns**
    - Proven patterns from other financial clients (IDP flows, email-to-case, exception handling).

**Key line:**

> “Inside the thin layer, we embed **EY assets like an agent test harness**, so every agent can be validated before go-live. This makes the platform feel like a product on day one, not an empty shell.”

Where it maps:

- Builder: “Test & Validate” as part of the build flow.
- Platform operations: regression testing & quality gates.

---

### 4.3 Templates – Accelerating From Proven Patterns

On top of the thin client and assets, we give the client a **template catalog** so teams don’t start from scratch.

Three types of templates:

1. **Use-Case Templates**
    - Email-to-case triage.
    - Document review & extraction with approvals.
    - Exception / break handling flows.

2. **Agent Templates**
    - Classification agent.
    - Summarization + routing agent.
    - Investigation / companion agent.

3. **Governance & Ops Templates**
    - Standard roles & approval patterns.
    - Human-in-the-loop configurations.
    - Cost/usage & quality dashboards.

**Key line:**

> “The thin client doesn’t come empty – it ships with a **catalog of templates** based on what we’ve already proven at other financial institutions. Teams start from patterns, not a blank screen.”

Where it maps:

- Builder Layer (no-code builder + template gallery).
- Conceptually an internal **Marketplace** of agents and flows.

---

## 5. Act 3 – How It Fits Into Our 7-Layer Platform Model

To keep everyone aligned, we summarize the platform as **7 layers**.  
This is the “mental model” we’ll use across architecture, RFP text, and slides.

### 5.1 The 7 Layers (WHAT, Not HOW)

1. **Experience Layer – How people interact**
    - Thin client / portal for business users, developers, and admins.
    - Views for agents, runs, exceptions, approvals.

2. **Builder Layer – How agents & workflows are created**
    - No-code / low-code workflow and agent builder.
    - Prompt and tool configuration.
    - Template catalog (use cases, agents, governance patterns).
    - Integrated **agent test harness** (Test & Validate).

3. **Runtime Layer – Where agents execute**
    - **Cloud-native, model-agnostic runtime** (no vendor hard-wiring in the business logic).
    - Agents call a **model gateway**, not directly a single model.
    - Runtime can route to different approved models/providers over time.
    - Handles scaling, state, sessions, reliability.

4. **Integration & Tools Layer – How agents talk to systems**
    - Connectors to enterprise systems: email, ticketing, core platforms, data, SaaS.
    - Reusable tools/actions (APIs, tasks) that agents can invoke.
    - Event ingestion (documents, emails, tickets, streams) as triggers.

5. **Knowledge & Memory Layer – What agents know and remember**
    - Controlled access to documents, structured data, knowledge bases.
    - Document understanding + retrieval.
    - Short-term and long-term memory for agents where appropriate.

6. **Governance & Control Layer – How we keep it safe**
    - Identity, roles, permissions.
    - Policies & guardrails (data usage, model usage, safety).
    - Human-in-the-loop rules and approval workflows.
    - Audit trails for configuration and agent actions.

7. **Platform Operations Layer – How we run this as an enterprise platform**
    - Monitoring, logging, and health.
    - Quality and performance metrics.
    - **Agent evaluation & regression test harness** (quality gates).
    - Cost/usage insights and lifecycle management (sandbox → pilot → prod).

---

### 5.2 Short Talk Track Linking the Story to the 7 Layers

This is what someone on the team can actually **say**:

> “We structure everything into **seven layers**.  
> At the top, the **Experience Layer** is our thin client – one portal for business, developers, and admins to see and manage agents.
>
> The **Builder Layer** is where they design workflows and agents in a no-code way. This is also where we surface our **templates** and our **agent test harness**, so they can start from proven patterns and validate every change before it goes live.
>
> Underneath that, a **cloud-native, model-agnostic Runtime Layer** executes agents and workflows using a model gateway – so they can change models and providers over time without redesigning processes.
>
> The **Integration & Tools Layer** connects agents to real systems and data; the **Knowledge & Memory Layer** makes sure agents are grounded in the right information; the **Governance & Control Layer** bakes in identity, policies, and human-in-the-loop; and the **Platform Operations Layer** covers monitoring, quality, regression testing, and cost.
>
> Together, this gives the client a standard, governed way to scale AI agents – with a light footprint on top of their existing cloud.”

---
