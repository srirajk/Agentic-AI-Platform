# Complete User Journey Flow

## Overview
This document shows the complete user journey through the AI Agentic Platform, from initial entry through profile selection, workspace provisioning, and interaction with different studio environments.

---

## High-Level Journey Map

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                                                                             │
│                        USER ENTERS PLATFORM                                 │
│                                                                             │
└───────────────────────────────────┬─────────────────────────────────────────┘
                                    │
                                    ↓
┌───────────────────────────────────────────────────────────────────────────┐
│  SCREEN 01: LANDING PAGE - PROFILE SELECTION                              │
│  ────────────────────────────────────────────────────────────────────────  │
│                                                                            │
│  User sees 4 persona cards:                                               │
│  • 📊 Data Scientist      • 🔧 Low-Code Builder                           │
│  • 📝 Declarative Builder • 📈 Business Analyst                           │
│                                                                            │
│  Decision: Select a profile OR choose recent workspace                    │
│                                                                            │
└────────┬──────────────────────────┬──────────────────────────┬─────────────┘
         │                          │                          │
         ↓                          ↓                          ↓
    New Profile              Recent Workspace          First-Time User
    Selection                Quick Access              (Show Tutorial)
         │                          │                          │
         ↓                          ↓                          ↓
┌─────────────────────┐   ┌──────────────────────┐   ┌──────────────────┐
│  SCREEN 02:         │   │  SCREEN 02:          │   │  Onboarding      │
│  WORKSPACE          │   │  WORKSPACE           │   │  Wizard          │
│  PROVISIONING       │   │  PROVISIONING        │   │  (Optional)      │
│  (New Setup)        │   │  (Restore Session)   │   │                  │
│                     │   │                      │   │  • Platform tour │
│  Progress:          │   │  Progress:           │   │  • Quick start   │
│  ✓ Initialize       │   │  ✓ Load state        │   │  • Video guide   │
│  ✓ Load studio      │   │  ⟳ Restore files     │   │                  │
│  ⟳ Configure        │   │  ○ Reconnect         │   └─────┬────────────┘
│  ○ Prepare cat.     │   │                      │          │
│  ○ Setup collab     │   │  Faster (~5-10s)     │          │
│                     │   │                      │          │
│  (~15-20s)          │   └──────────┬───────────┘          │
│                     │              │                      │
└──────────┬──────────┘              │                      │
           │                         │                      │
           └─────────────────────────┴──────────────────────┘
                                     │
                                     ↓
┌───────────────────────────────────────────────────────────────────────────┐
│  SCREEN 03: MAIN DASHBOARD (Unified Hub)                                 │
│  ────────────────────────────────────────────────────────────────────────  │
│                                                                            │
│  Central hub showing:                                                     │
│  • All 4 studio environments (regardless of initial profile)              │
│  • Recent activity across studios                                        │
│  • Shared resources (Tool Catalogue, Templates, etc.)                    │
│                                                                            │
│  User can:                                                                │
│  • Switch to any studio                                                   │
│  • Continue recent work                                                   │
│  • Browse catalogue                                                       │
│  • Access documentation                                                   │
│                                                                            │
└────┬──────────┬─────────────┬─────────────┬──────────────────────────────┘
     │          │             │             │
     ↓          ↓             ↓             ↓
┌─────────┐ ┌────────┐ ┌────────────┐ ┌──────────┐
│ Screen  │ │ Screen │ │ Screen     │ │ Screen   │
│ 04      │ │ 05     │ │ 06         │ │ 07       │
│         │ │        │ │            │ │          │
│ Data    │ │ Low-   │ │ Declarative│ │ Business │
│ Science │ │ Code   │ │ Builder    │ │ Analyst  │
│ Studio  │ │ Studio │ │            │ │ Studio   │
└────┬────┘ └───┬────┘ └──────┬─────┘ └─────┬────┘
     │          │             │             │
     └──────────┴─────────────┴─────────────┘
                      │
                      ↓
        Can return to Dashboard anytime
        via breadcrumb or menu
```

---

## Detailed Flow by Persona

### Persona 1: Data Scientist Journey

```
Landing Page (Screen 01)
    ↓
[Selects "Data Scientist"]
    ↓
Provisioning (Screen 02)
    • Initialize workspace container
    • Load Jupyter environment
    • Connect to SageMaker
    • Prepare ML tools catalogue
    ↓
Main Dashboard (Screen 03)
    • Shows Data Science studio as "active"
    • Other studios available
    • Recent notebooks listed
    ↓
[Clicks "Continue Working" on Data Science Studio]
    ↓
Data Science Studio (Screen 04)
    │
    ├─ Open Notebook
    │   • customer_churn_model.ipynb
    │   • Execute cells
    │   • View outputs
    │
    ├─ Use Tool Catalogue (Right Panel)
    │   • Search "transformers"
    │   • View BERT model details
    │   • Click "Insert Code Snippet"
    │   • Code added to active cell
    │
    ├─ Train Model
    │   • Switch to Training Dashboard view
    │   • Monitor progress
    │   • View metrics (loss, accuracy)
    │
    └─ Optional: Switch Studio
        • Click "Studios ▼" dropdown
        • Select "Low-Code Studio"
        • Returns to Dashboard → Routes to Low-Code
```

---

### Persona 2: Low-Code Builder Journey

```
Landing Page (Screen 01)
    ↓
[Selects "Low-Code Builder"]
    ↓
Provisioning (Screen 02)
    • Initialize workspace
    • Load n8n-style editor
    • Connect to integration hub
    • Prepare node catalogue
    ↓
Main Dashboard (Screen 03)
    • Shows Low-Code studio as "active"
    • Recent workflows listed
    ↓
[Clicks "Continue Working" on Low-Code Studio]
    ↓
Low-Code Studio (Screen 05)
    │
    ├─ Create New Workflow
    │   • Blank canvas appears
    │   • Drag "Webhook" trigger node from left panel
    │   • Configure webhook endpoint
    │
    ├─ Use Tool Catalogue (Right Panel)
    │   • Browse "AI/LLM Nodes"
    │   • Drag "OpenAI GPT-4" to canvas
    │   • Connect Webhook → OpenAI node
    │
    ├─ Add Logic & Actions
    │   • Add "Condition" node
    │   • Add "Email" and "Slack" output nodes
    │   • Connect all nodes
    │
    ├─ Configure Nodes
    │   • Click each node
    │   • Fill configuration modal
    │   • Test individual nodes
    │
    ├─ Test Workflow
    │   • Click "Test" button
    │   • View execution log
    │   • Debug if errors
    │
    └─ Deploy
        • Click "Deploy" button
        • Workflow goes live
        • Returns to Dashboard
```

---

### Persona 3: Declarative Builder Journey

```
Landing Page (Screen 01)
    ↓
[Selects "Declarative Builder"]
    ↓
Provisioning (Screen 02)
    • Initialize workspace
    • Load form-based builder
    • Prepare agent templates
    • Connect to prompt library
    ↓
Main Dashboard (Screen 03)
    • Shows Declarative Builder as "active"
    • Recent agents listed
    ↓
[Clicks "Launch Studio" on Declarative Builder]
    ↓
Declarative Builder (Screen 06)
    │
    ├─ Load Template (Optional)
    │   • Click "Load Template" in catalogue panel
    │   • Browse "Sales Assistant" template
    │   • Click to pre-fill form
    │
    ├─ Step 1: Basic Information
    │   • Enter agent name
    │   • Write description
    │   • Select agent type (Chat Agent)
    │   • Choose primary goal
    │   • Set tone/personality
    │
    ├─ Step 2: Model Configuration
    │   • Select "OpenAI"
    │   • Choose "GPT-4 Turbo"
    │   • Adjust temperature slider
    │   • Set max tokens
    │   • View cost estimate
    │
    ├─ Step 3: Prompt Engineering
    │   • Write system prompt
    │   • Define user message template
    │   • Add few-shot examples
    │
    ├─ Step 4: Tools & Integrations
    │   • Check "Product Search"
    │   • Check "Inventory Check"
    │   • Configure each tool
    │
    ├─ Step 5: Memory & Context
    │   • Select "Short-term memory"
    │   • Upload "Product Catalog" knowledge base
    │   • Configure RAG settings
    │
    ├─ Step 6: Guardrails & Safety
    │   • Enable profanity filter
    │   • Set topic boundaries
    │   • Configure fallback actions
    │
    ├─ Step 7: Review & Deploy
    │   • Review configuration summary
    │   • Check validation status
    │   • Click "Test Agent"
    │   • Interactive chat preview appears
    │   • Test conversation
    │   • View debug logs
    │   • Click "Deploy to Staging"
    │
    └─ Post-Deployment
        • Returns to Dashboard
        • Agent appears in "Recent Activity"
        • Can monitor via Business Analytics
```

---

### Persona 4: Business Analyst Journey

```
Landing Page (Screen 01)
    ↓
[Selects "Business Analyst"]
    ↓
Provisioning (Screen 02)
    • Initialize workspace
    • Load analytics environment
    • Connect to data sources
    • Prepare visualization tools
    ↓
Main Dashboard (Screen 03)
    • Shows Business Analytics as "active"
    • Recent dashboards listed
    ↓
[Clicks "Continue Working" on Business Analytics]
    ↓
Business Analytics Studio (Screen 07)
    │
    ├─ View Pre-built Dashboard
    │   • "Agent Performance Overview" loads
    │   • Key metrics cards display
    │   • Charts show trends
    │   • AI insights highlighted
    │
    ├─ Apply Filters
    │   • Change time range to "Last 30 Days"
    │   • Filter by agent: "Sales_Assistant"
    │   • Click "Apply Filters"
    │   • Dashboard updates
    │
    ├─ Drill Down
    │   • Click on "Query Volume" chart
    │   • Detailed breakdown appears
    │   • Export data to Excel
    │
    ├─ Create Custom Report
    │   • Click "New Report"
    │   • Query Builder modal opens
    │   • Select data source: "Agent Logs"
    │   • Choose metrics: Cost, Query Count
    │   • Apply filters
    │   • Group by Agent Name
    │   • Select visualization: Bar Chart
    │   • Click "Preview"
    │   • Review chart
    │   • Click "Save as Dashboard"
    │
    ├─ Use Natural Language Query
    │   • Click "Ask a Question"
    │   • Type: "Which agent costs the most?"
    │   • AI generates answer with data
    │   • Click "Create Report" to save
    │
    ├─ Set Up Alert
    │   • Navigate to "Alerts" in left panel
    │   • Click "Create Alert"
    │   • Configure: "Success Rate < 90%"
    │   • Set notification: Email + Slack
    │   • Enable auto-actions
    │   • Save alert
    │
    └─ Schedule Report
        • Select dashboard
        • Click "Schedule Report"
        • Set frequency: "Weekly"
        • Add recipients
        • Choose format: PDF
        • Save schedule
```

---

## Cross-Studio Workflows

### Workflow 1: Data Scientist → Business Analyst

```
User in Data Science Studio (Screen 04)
    ↓
Trains new ML model
    ↓
Clicks "Studios ▼" → Selects "Business Analytics"
    ↓
Routes to Main Dashboard (Screen 03)
    ↓
Clicks "Business Analytics Studio"
    ↓
Business Analytics Studio (Screen 07)
    ↓
Creates report on model performance
    ↓
Shares dashboard with team
```

---

### Workflow 2: Declarative Builder → Low-Code Builder

```
User in Declarative Builder (Screen 06)
    ↓
Creates basic chat agent using forms
    ↓
Realizes need for complex workflow logic
    ↓
Clicks "Studios ▼" → Selects "Low-Code Studio"
    ↓
Routes to Main Dashboard (Screen 03)
    ↓
Clicks "Low-Code Studio"
    ↓
Low-Code Studio (Screen 05)
    ↓
Imports declarative agent as a node
    ↓
Builds workflow around it with additional logic
    ↓
Deploys combined solution
```

---

### Workflow 3: Business Analyst → Declarative Builder

```
User in Business Analytics (Screen 07)
    ↓
Identifies underperforming agent via report
    ↓
Clicks agent name → "Optimize Agent"
    ↓
Routes to Declarative Builder (Screen 06)
    ↓
Agent configuration loads
    ↓
Adjusts prompt and settings
    ↓
Tests improved agent
    ↓
Deploys update
    ↓
Returns to Analytics to monitor improvement
```

---

## Tool Catalogue Integration Flow

The Tool Catalogue (Screen 08) is accessible from ALL studios:

```
User in ANY Studio (04/05/06/07)
    │
    ├─ Right Panel: Catalogue Always Visible
    │   │
    │   ├─ Browse Categories
    │   │   • Expand "AI/LLM Models"
    │   │   • See GPT-4, Claude, etc.
    │   │
    │   ├─ Search
    │   │   • Type "openai"
    │   │   • Filter results appear
    │   │
    │   ├─ View Details
    │   │   • Click "View" on item
    │   │   • Detail modal opens
    │   │   • Read description, pricing, features
    │   │   • View code examples
    │   │
    │   ├─ Add to Project
    │   │   • Click "Add to Project"
    │   │   • Item integrated into current studio
    │   │   │
    │   │   │ Context-aware integration:
    │   │   ├─ Data Science: Package installed
    │   │   ├─ Low-Code: Node added to palette
    │   │   ├─ Declarative: Config option appears
    │   │   └─ Analytics: Data source connected
    │   │
    │   ├─ Favorites
    │   │   • Click star icon
    │   │   • Added to Favorites list
    │   │   • Quick access in future
    │   │
    │   └─ Full Catalogue View
    │       • Click "View Full Catalogue"
    │       • Modal with grid of all items
    │       • Advanced filtering
    │       • Browse by category
    │       • Sort by popularity, price, etc.
    │
    └─ Catalogue panel collapses if needed
        • More canvas space
        • Quick toggle to re-open
```

---

## Navigation Patterns

### Breadcrumb Navigation (Always Available)

```
Home > My Workspace > [Current Studio]
  │         │              │
  ↓         ↓              ↓
 Back to  Back to      Current
 Landing  Dashboard    Location
```

### Studio Switcher Dropdown (Always Available)

```
[≡ Studios ▼]
  │
  ├─ 📊 Data Science Studio
  ├─ 🔧 Low-Code Studio
  ├─ 📝 Declarative Builder
  ├─ 📈 Business Analytics
  │
  └─ [Switch Studio]
      │
      ↓
  Saves current work
      ↓
  Returns to Dashboard
      ↓
  Routes to selected studio
```

---

## Key User Journeys Summary

### Journey A: Complete Beginner (Non-Technical)
```
Landing → Declarative Builder → Build simple agent via forms
       → Test agent → Deploy → View analytics
```

### Journey B: Technical User (Developer/Data Scientist)
```
Landing → Data Science Studio → Code ML models in notebooks
       → Switch to Low-Code → Wrap model in workflow
       → Deploy → Monitor via Analytics
```

### Journey C: Business User
```
Landing → Business Analytics → View pre-built dashboards
       → Create custom reports → Set up alerts
       → Share with team
```

### Journey D: Power User (Uses All Studios)
```
Landing → Dashboard → Start in Data Science
       → Train model → Switch to Low-Code
       → Build workflow → Switch to Declarative
       → Configure agent → Switch to Analytics
       → Monitor performance → Optimize → Repeat
```

---

## Mobile/Responsive Journey

On mobile devices, the experience adapts:

1. **Landing Page**: Cards stack vertically
2. **Dashboard**: Studios displayed as list
3. **Studios**:
   - Catalogue panel becomes bottom sheet
   - Canvas/workspace takes full width
   - Toggle between workspace and catalogue
4. **Navigation**: Hamburger menu for studio switching

---

## Error & Edge Cases

### Error Recovery Flow
```
User action triggers error
    ↓
Error notification appears
    ↓
User options:
    ├─ Retry action
    ├─ Report issue
    ├─ View error details
    └─ Return to safe state (Dashboard)
```

### Session Timeout
```
User inactive for 30+ minutes
    ↓
Auto-save triggered
    ↓
Session warning appears: "5 minutes until timeout"
    ↓
User can:
    ├─ Continue working (extends session)
    └─ Allow timeout
        ↓
    Redirects to Landing
        ↓
    Work preserved, can resume
```

---

## Design Principles Reflected in Journey

1. **Progressive Disclosure**: Start simple (profile selection) → expand complexity (studio features)
2. **Flexibility**: Users can switch studios anytime, not locked into initial choice
3. **Consistency**: Tool catalogue, navigation, and patterns consistent across studios
4. **Context Preservation**: Work saved when switching, can resume anywhere
5. **Guided Assistance**: Tooltips, templates, AI insights guide users
6. **Performance**: Fast transitions, background loading, optimistic UI updates
7. **Accessibility**: Keyboard navigation, ARIA labels, screen reader support throughout
