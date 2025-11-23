# Declarative Agent Builder Studio

## Screen Purpose
Form-based, template-driven interface for configuring AI agents without any coding. Users fill out forms and select options to create production-ready agents.

---

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
│  AI AGENTIC PLATFORM                                                     [User: John]  [Settings] ⚙        │
├─────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
│  Home > My Workspace > Declarative Builder                                                                  │
│                                                                                                              │
│  ┌────────────────────────────────────────────────────────────────────────────────────┐                     │
│  │  📝 DECLARATIVE BUILDER    Agent: Sales_Assistant_v2      [≡ Studios ▼]           │                     │
│  │  [💾 Save Draft]  [👁 Preview]  [🧪 Test Agent]  [✓ Validate]  [↗ Deploy]        │                     │
│  └────────────────────────────────────────────────────────────────────────────────────┘                     │
│                                                                                                              │
│  ┌──────────┬──────────────────────────────────────────────────────────────────────┬────────────────────────┐│
│  │ CONFIG   │                AGENT CONFIGURATION FORM                              │  TOOL CATALOGUE       ││
│  │ STEPS    │                                                                       │  ─────────────────    ││
│  ├──────────┤                                                                       │                       ││
│  │          │  ┌───────────────────────────────────────────────────────────────┐   │  🔍 Search...         ││
│  │ ✓ 1.     │  │  STEP 1: BASIC INFORMATION                               [▼] │   │  ─────────────────    ││
│  │   Basic  │  ├───────────────────────────────────────────────────────────────┤   │                       ││
│  │   Info   │  │                                                               │   │  📋 Templates (45)    ││
│  │          │  │  Agent Name: [Sales_Assistant_v2                         ]   │   │  ├─ Customer Support   ││
│  │ → 2.     │  │                                                               │   │  ├─ Sales Assistant   ││
│  │   Model  │  │  Description:                                                 │   │  ├─ Data Analyst      ││
│  │   Setup  │  │  ┌────────────────────────────────────────────────────────┐  │   │  ├─ Content Creator   ││
│  │          │  │  │ An AI sales assistant that helps customers find       │  │   │  └─ Research Agent    ││
│  │ ○ 3.     │  │  │ products, answer questions, and complete purchases.   │  │   │                       ││
│  │   Prompt │  │  │                                                        │  │   │  🤖 Agent Roles (28)  ││
│  │          │  │  └────────────────────────────────────────────────────────┘  │   │  ├─ Conversational    ││
│  │ ○ 4.     │  │                                                               │   │  ├─ Analytical        ││
│  │   Tools  │  │  Agent Type: ● Chat Agent  ○ Task Agent  ○ Multi-Agent      │   │  ├─ Creative          ││
│  │          │  │                                                               │   │  └─ Specialized       ││
│  │ ○ 5.     │  │  Primary Goal: [Assist customers with product selection ▼]  │   │                       ││
│  │   Memory │  │                                                               │   │  🧩 Components (67)   ││
│  │          │  │  Tone/Personality: [Professional and Friendly           ▼]  │   │  ├─ Memory Systems     ││
│  │ ○ 6.     │  │                                                               │   │  ├─ Tool Integrations ││
│  │   Guard  │  └───────────────────────────────────────────────────────────────┘   │  ├─ Prompt Templates  ││
│  │   rails  │                                                                       │  └─ Guardrails        ││
│  │          │  ┌───────────────────────────────────────────────────────────────┐   │                       ││
│  │ ○ 7.     │  │  STEP 2: MODEL CONFIGURATION                             [▼] │   │  🔌 Integrations(89)  ││
│  │   Review │  ├───────────────────────────────────────────────────────────────┤   │  ├─ CRM Systems        ││
│  │          │  │                                                               │   │  ├─ E-commerce        ││
│  │          │  │  Language Model:                                              │   │  ├─ Databases         ││
│  │          │  │  ● OpenAI    ○ Anthropic    ○ Cohere    ○ Custom            │   │  └─ APIs              ││
│  │          │  │                                                               │   │                       ││
│  │          │  │  Model Version: [GPT-4 Turbo                             ▼] │   │  ─────────────────    ││
│  │          │  │                                                               │   │                       ││
│  │          │  │  Model Parameters:                                            │   │  [View Catalogue]     ││
│  │          │  │  ┌─────────────────────────────────────────────────────────┐ │   │                       ││
│  │          │  │  │ Temperature:    [0.7          ] ←────→  (0 = Focused)  │ │   │  QUICK ACTIONS        ││
│  │          │  │  │                                          (1 = Creative) │ │   │  ─────────────────    ││
│  │          │  │  │ Max Tokens:     [2000         ]                         │ │   │                       ││
│  │          │  │  │                                                         │ │   │  [📋 Load Template]   ││
│  │          │  │  │ Top P:          [0.9          ]                         │ │   │  [💾 Save Template]   ││
│  │          │  │  │                                                         │ │   │  [📂 My Agents]       ││
│  │          │  │  │ Frequency Pen.: [0.0          ]                         │ │   │  [🔄 Clone Agent]     ││
│  │          │  │  └─────────────────────────────────────────────────────────┘ │   │                       ││
│  │          │  │                                                               │   │  VALIDATION           ││
│  │          │  │  Fallback Model: [GPT-3.5 Turbo (if primary fails)      ▼] │   │  ─────────────────    ││
│  │          │  │                                                               │   │                       ││
│  │          │  │  Cost Estimation: ~$0.03 per conversation (based on avg)    │   │  ✓ Basic Info         ││
│  │          │  │                                                               │   │  ✓ Model Setup        ││
│  │          │  └───────────────────────────────────────────────────────────────┘   │  ⚠ Prompt needed      ││
│  │          │                                                                       │  ○ Tools pending      ││
│  │          │  [Collapse All]  [Expand All]                                        │  ○ Memory pending     ││
│  │ Click    │                                                                       │  ○ Guardrails pending ││
│  │ step to  │                                                                       │                       ││
│  │ jump     │                                                                       │  Progress: 28%        ││
│  │   ↑      │                                                                       │  ████░░░░░░░░         ││
│  │          │                                                                       │                       ││
│  └──────────┴───────────────────────────────────────────────────────────────────────┴────────────────────────┘│
│                                                                                                              │
│  ┌────────────────────────────────────────────────────────────────────────────────────────────────────────┐ │
│  │  💡 HELPFUL TIPS                                                                                       │ │
│  │  ────────────────────────────────────────────────────────────────────────────────────────────────────  │ │
│  │  • Choose GPT-4 for complex reasoning, GPT-3.5 for faster responses                                   │ │
│  │  • Lower temperature (0.3-0.5) for factual tasks, higher (0.7-0.9) for creative tasks                 │ │
│  │  [View Full Documentation] [Watch Tutorial Video]                                                     │ │
│  └────────────────────────────────────────────────────────────────────────────────────────────────────────┘ │
│                                                                                                              │
└─────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Configuration Steps Overview

### Step 1: Basic Information ✓
- Agent name
- Description
- Agent type (Chat/Task/Multi-Agent)
- Primary goal selection
- Tone/personality

### Step 2: Model Configuration → (Currently Viewing)
- LLM provider selection (OpenAI, Anthropic, etc.)
- Model version
- Temperature, tokens, and other parameters
- Fallback model
- Cost estimation

### Step 3: Prompt Engineering ○
```
┌───────────────────────────────────────────────────────────┐
│  STEP 3: PROMPT CONFIGURATION                        [▼] │
├───────────────────────────────────────────────────────────┤
│                                                           │
│  System Prompt:                                           │
│  ┌───────────────────────────────────────────────────┐   │
│  │ You are a friendly sales assistant for TechCorp.  │   │
│  │ Your goal is to help customers find the right    │   │
│  │ products by understanding their needs.            │   │
│  │                                                   │   │
│  │ Key Guidelines:                                   │   │
│  │ - Always greet customers warmly                  │   │
│  │ - Ask clarifying questions to understand needs   │   │
│  │ - Provide max 3 product recommendations          │   │
│  │ - Include prices and key features                │   │
│  └───────────────────────────────────────────────────┘   │
│                                                           │
│  [Load from Template ▼]  [Test Prompt]                   │
│                                                           │
│  User Message Template:                                   │
│  ┌───────────────────────────────────────────────────┐   │
│  │ Customer Query: {{user_input}}                    │   │
│  │ Customer History: {{customer_data}}               │   │
│  │ Available Products: {{product_catalog}}           │   │
│  └───────────────────────────────────────────────────┘   │
│                                                           │
│  Few-Shot Examples: [+ Add Example]                      │
│  1. Q: "I need a laptop for coding"                      │
│     A: "Great! For coding, I'd recommend..."             │
│  2. [+ Add more examples]                                 │
│                                                           │
└───────────────────────────────────────────────────────────┘
```

### Step 4: Tools & Integrations ○
```
┌───────────────────────────────────────────────────────────┐
│  STEP 4: TOOLS & CAPABILITIES                        [▼] │
├───────────────────────────────────────────────────────────┤
│                                                           │
│  Available Tools: (Select tools your agent can use)      │
│                                                           │
│  ☑ Product Search                                        │
│    Search product catalog by keywords, filters           │
│    [Configure ⚙]                                          │
│                                                           │
│  ☑ Inventory Check                                       │
│    Check real-time product availability                  │
│    [Configure ⚙]                                          │
│                                                           │
│  ☑ Price Calculator                                      │
│    Calculate totals, apply discounts, estimate shipping  │
│    [Configure ⚙]                                          │
│                                                           │
│  ☐ Order Placement                                       │
│    Create orders in e-commerce system                    │
│    [Configure ⚙]                                          │
│                                                           │
│  ☐ Customer Database Access                              │
│    Retrieve customer history and preferences             │
│    [Configure ⚙]                                          │
│                                                           │
│  [+ Add Tool from Catalogue]                             │
│                                                           │
│  Custom Functions:                                        │
│  [+ Add Custom Function]                                  │
│                                                           │
└───────────────────────────────────────────────────────────┘
```

### Step 5: Memory & Context ○
```
┌───────────────────────────────────────────────────────────┐
│  STEP 5: MEMORY CONFIGURATION                        [▼] │
├───────────────────────────────────────────────────────────┤
│                                                           │
│  Conversation Memory:                                     │
│  ● Short-term (session only)                             │
│  ○ Long-term (persist across sessions)                   │
│  ○ Hybrid (short + long term)                            │
│                                                           │
│  Memory Window: [10 messages ▼]                          │
│  (How many previous messages to remember)                │
│                                                           │
│  Knowledge Base:                                          │
│  ☑ Product Catalog (1,234 items)                         │
│  ☑ FAQ Document (89 Q&As)                                │
│  ☐ Company Policies (PDF)                                │
│  [+ Upload Knowledge Base]                                │
│                                                           │
│  RAG Configuration:                                       │
│  Embedding Model: [text-embedding-ada-002 ▼]             │
│  Chunk Size: [500 tokens]                                │
│  Top K Results: [3]                                      │
│                                                           │
│  [Advanced Settings ▼]                                    │
│                                                           │
└───────────────────────────────────────────────────────────┘
```

### Step 6: Guardrails & Safety ○
```
┌───────────────────────────────────────────────────────────┐
│  STEP 6: GUARDRAILS & SAFETY                         [▼] │
├───────────────────────────────────────────────────────────┤
│                                                           │
│  Content Filtering:                                       │
│  ☑ Profanity filter                                      │
│  ☑ PII detection & redaction                             │
│  ☑ Harmful content blocking                              │
│                                                           │
│  Topic Boundaries:                                        │
│  Allowed Topics:                                          │
│  • Product information                                    │
│  • Pricing and availability                              │
│  • General shopping assistance                           │
│                                                           │
│  Restricted Topics:                                       │
│  • Medical advice                                         │
│  • Legal advice                                           │
│  • Financial planning                                     │
│  [+ Add Topic]                                            │
│                                                           │
│  Response Validation:                                     │
│  ☑ Factual accuracy check (via knowledge base)           │
│  ☑ Brand voice consistency                               │
│  ☐ Human review for sensitive topics                     │
│                                                           │
│  Fallback Actions:                                        │
│  If agent uncertain: [Route to human agent ▼]            │
│  If topic restricted: [Show canned response ▼]           │
│                                                           │
└───────────────────────────────────────────────────────────┘
```

### Step 7: Review & Deploy ○
```
┌───────────────────────────────────────────────────────────┐
│  STEP 7: REVIEW & DEPLOY                             [▼] │
├───────────────────────────────────────────────────────────┤
│                                                           │
│  Configuration Summary:                                   │
│                                                           │
│  Agent Name: Sales_Assistant_v2                           │
│  Type: Chat Agent                                         │
│  Model: GPT-4 Turbo                                       │
│  Tools: 3 enabled                                         │
│  Memory: Short-term (10 messages)                         │
│  Guardrails: ✓ Enabled                                   │
│                                                           │
│  Validation Status:                                       │
│  ✓ All required fields completed                         │
│  ✓ Configuration is valid                                │
│  ✓ Tools properly configured                             │
│  ⚠ Warning: No fallback model configured                 │
│                                                           │
│  Cost Estimate: $0.03/conversation (avg)                 │
│                                                           │
│  Testing:                                                 │
│  ☑ Passed basic conversation test                        │
│  ☑ Passed tool invocation test                           │
│  ☐ Human QA review pending                               │
│                                                           │
│  Deployment Options:                                      │
│  ● Deploy to staging first                               │
│  ○ Deploy directly to production                         │
│                                                           │
│  [◄ Back to Edit]    [🧪 Test Again]    [↗ Deploy]       │
│                                                           │
└───────────────────────────────────────────────────────────┘
```

---

## Tool Catalogue Panel - Expanded

```
┌───────────────────────────┐
│  TOOL CATALOGUE          │
│  ─────────────────       │
│                          │
│  🔍 Search templates...  │
│  ─────────────────       │
│                          │
│  📋 Templates (45) [▼]   │
│  ├─ Customer Support     │
│  │   ├─ Email Support    │ ← Click to load
│  │   ├─ Chat Support     │
│  │   └─ Ticket Routing   │
│  ├─ Sales Assistant      │
│  │   ├─ Lead Qualifier   │
│  │   ├─ Product Advisor  │
│  │   └─ Upsell Agent     │
│  ├─ Data Analyst         │
│  └─ Content Creator      │
│                          │
│  🤖 Agent Roles [▶]      │
│                          │
│  🧩 Components [▶]       │
│                          │
│  🔌 Integrations [▶]     │
│                          │
│  ─────────────────       │
│                          │
│  [View Full Catalogue]   │
│                          │
│  QUICK ACTIONS           │
│  ─────────────────       │
│                          │
│  [📋 Load Template]      │
│  [💾 Save Template]      │
│  [📂 My Agents]          │
│  [🔄 Clone Agent]        │
│                          │
│  VALIDATION              │
│  ─────────────────       │
│                          │
│  ✓ Basic Info            │
│  ✓ Model Setup           │
│  ⚠ Prompt needed         │
│  ○ Tools pending         │
│  ○ Memory pending        │
│  ○ Guardrails pending    │
│                          │
│  Progress: 28%           │
│  ████░░░░░░░░            │
│                          │
└───────────────────────────┘
```

---

## Preview/Test Agent Panel

Click "Preview" or "Test Agent":

```
┌─────────────────────────────────────────────────────────────┐
│  Test Agent: Sales_Assistant_v2                       [✕]  │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ┌─────────────────────────────────────────────────────┐   │
│  │  💬 Chat Preview                                    │   │
│  ├─────────────────────────────────────────────────────┤   │
│  │                                                     │   │
│  │  🤖 Sales Assistant:                                │   │
│  │  Hello! I'm here to help you find the perfect      │   │
│  │  products. What are you looking for today?         │   │
│  │                                                     │   │
│  │  👤 You:                                            │   │
│  │  I need a laptop for software development          │   │
│  │                                                     │   │
│  │  🤖 Sales Assistant:                                │   │
│  │  Great choice! For software development, I'd        │   │
│  │  recommend these options:                           │   │
│  │                                                     │   │
│  │  1. MacBook Pro 16" M3 - $2,499                    │   │
│  │     • 36GB RAM, 512GB SSD                          │   │
│  │     • Best for iOS/Mac development                 │   │
│  │                                                     │   │
│  │  🔧 [Tool Used: Product Search]                    │   │
│  │  🔧 [Tool Used: Inventory Check]                   │   │
│  │                                                     │   │
│  └─────────────────────────────────────────────────────┘   │
│                                                             │
│  Type your message: [                              ]  [→]  │
│                                                             │
│  [Reset Chat]  [View Debug Logs]  [Export Conversation]   │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## User Interactions

### 1. Configuration Workflow
- **Linear Steps**: Follow 7 steps from Basic Info to Deploy
- **Jump to Step**: Click step in left sidebar to skip ahead
- **Expand/Collapse**: Toggle sections for focused editing
- **Auto-save**: Configuration saved automatically every 30s

### 2. Tool Catalogue Integration
- **Load Template**: Pre-fill form with template values
- **Add Components**: Drag or click to add tools/integrations
- **Clone Agent**: Duplicate existing agent as starting point
- **Save as Template**: Save current config for reuse

### 3. Validation
- **Real-time Checks**: Validate fields as user types
- **Progress Tracking**: Visual indicator of completion %
- **Error Highlighting**: Red indicators for missing/invalid fields
- **Warnings**: Yellow alerts for recommendations

### 4. Testing
- **Preview Mode**: See how agent will respond
- **Test Conversations**: Interactive chat to validate behavior
- **Debug Logs**: View internal reasoning and tool calls
- **Performance Metrics**: Response time, cost per query

---

## Navigation Flow

```
Main Dashboard (Screen 03)
    ↓
[User clicks "Declarative Builder"]
    ↓
Declarative Builder (THIS SCREEN)
    │
    ├─ [New Agent] ──► Blank form (Step 1)
    ├─ [Load Template] ──► Pre-filled form
    ├─ [My Agents] ──► List of saved agents
    │
    └─ [Studios ▼] ──► Switch studio ──► Screen 04/05/07
```

---

## Design Notes

- **No Code Required**: Entirely form-based, accessible to non-technical users
- **Guided Experience**: Step-by-step wizard prevents overwhelm
- **Templates First**: Pre-built templates for common use cases
- **Smart Defaults**: Sensible default values for all parameters
- **Contextual Help**: Tooltips, tips, and documentation links throughout
- **Validation First**: Catch errors before deployment
- **Cost Transparency**: Show estimated costs upfront
- **Safe Deployment**: Staging environment before production
- **Rollback Support**: Version history to revert changes
- **Export Config**: Download agent config as JSON for version control
- **Collaboration**: Share agents with team members
- **Monitoring**: Post-deployment analytics on agent performance
