# Low-Code/No-Code Studio

## Screen Purpose
n8n-style visual workflow builder for creating AI agents and automation flows using drag-and-drop nodes.

---

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
│  AI AGENTIC PLATFORM                                                     [User: John]  [Settings] ⚙        │
├─────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
│  Home > My Workspace > Low-Code Studio                                                                      │
│                                                                                                              │
│  ┌────────────────────────────────────────────────────────────────────────────────────┐                     │
│  │  🔧 LOW-CODE STUDIO        Workflow: Customer_Support_Bot    [≡ Studios ▼]        │                     │
│  │  [💾 Save]  [▶ Execute]  [🧪 Test]  [📊 Analytics]  [⚙ Settings]  [↗ Deploy]     │                     │
│  └────────────────────────────────────────────────────────────────────────────────────┘                     │
│                                                                                                              │
│  ┌─────────┬────────────────────────────────────────────────────────────────────────┬──────────────────────┐│
│  │  NODES  │                     CANVAS / WORKFLOW BUILDER                          │  TOOL CATALOGUE     ││
│  │  PANEL  │                                                                         │  ─────────────────  ││
│  ├─────────┤                                                                         │                     ││
│  │         │     ┌──────────────┐                                                    │  🔍 Search...       ││
│  │ 🔵      │     │   TRIGGER    │                                                    │  ─────────────────  ││
│  │ Trigger │     │              │                                                    │                     ││
│  │         │     │  📨 Webhook  │                                                    │  📦 Nodes (156)     ││
│  │ 🟢      │     │  /support    │                                                    │  ├─ Triggers (12)   ││
│  │ Action  │     │              │                                                    │  ├─ AI/LLM (34)     ││
│  │         │     └──────┬───────┘                                                    │  ├─ Data (23)       ││
│  │ 🟡      │            │                                                            │  ├─ Logic (18)      ││
│  │ Logic   │            ↓                                                            │  ├─ Integration(45)  ││
│  │         │     ┌──────┴───────┐          ┌──────────────┐                         │  └─ Output (24)     ││
│  │ 🟣      │     │    AI NODE   │          │  CONDITION   │                         │                     ││
│  │ Data    │     │              │─────────→│              │                         │  🤖 Agent Lib (89)  ││
│  │         │     │  🤖 OpenAI   │          │  Priority?   │                         │  ├─ Chat Agents      ││
│  │ 🔴      │     │  GPT-4       │          │              │                         │  ├─ Task Agents      ││
│  │ AI/LLM  │     │              │          └──┬────────┬──┘                         │  ├─ RAG Agents       ││
│  │         │     └──────────────┘             │        │                            │  └─ Multi-Agent      ││
│  │ ⚙       │                                  │        │                            │                     ││
│  │ Config  │                        ┌─────────┘        └──────────┐                 │  🔌 Connectors(78)  ││
│  │         │                        ↓                             ↓                 │  ├─ Databases        ││
│  │         │              ┌─────────┴────────┐          ┌─────────┴────────┐        │  ├─ APIs             ││
│  │         │              │   HIGH PRIORITY  │          │   LOW PRIORITY   │        │  ├─ Cloud Services   ││
│  │         │              │                  │          │                  │        │  └─ Messaging        ││
│  │         │              │  📧 Email to     │          │  💬 Slack Msg    │        │                     ││
│  │         │              │     Agent        │          │     to Team      │        │  ─────────────────  ││
│  │         │              │                  │          │                  │        │                     ││
│  │ Drag    │              └──────────────────┘          └──────────────────┘        │  [View Catalogue]   ││
│  │ nodes   │                                                                         │                     ││
│  │ to      │                                                                         │  QUICK ACTIONS      ││
│  │ canvas  │                                                                         │  ─────────────────  ││
│  │   ↑     │                                                                         │                     ││
│  │   →     │                                                                         │  [+ Add Node]       ││
│  │         │                                                                         │  [📋 Templates]     ││
│  │         │                                                                         │  [⭐ Favorites]     ││
│  │         │                                                                         │  [📦 My Nodes]      ││
│  │         │                                                                         │                     ││
│  │         │                                                                         │  WORKFLOW INFO      ││
│  │         │                                                                         │  ─────────────────  ││
│  │         │                                                                         │                     ││
│  │         │                                                                         │  Nodes: 6           ││
│  │         │                                                                         │  Connections: 6     ││
│  │         │                                                                         │  Status: Draft      ││
│  │         │                                                                         │  Last run: Never    ││
│  │         │                                                                         │                     ││
│  └─────────┴─────────────────────────────────────────────────────────────────────────┴──────────────────────┘│
│                                                                                                              │
│  ┌────────────────────────────────────────────────────────────────────────────────────────────────────────┐ │
│  │  📊 EXECUTION LOG                                                                                      │ │
│  │  ────────────────────────────────────────────────────────────────────────────────────────────────────  │ │
│  │  No executions yet. Click "Execute" or "Test" to run this workflow.                                   │ │
│  │  [View Execution History]                                                                             │ │
│  └────────────────────────────────────────────────────────────────────────────────────────────────────────┘ │
│                                                                                                              │
└─────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Key Components

### 1. Studio Header
- **Workflow Name**: Current workflow being edited
- **Studios Dropdown**: Quick switch to other studios
- **Action Buttons**:
  - 💾 Save: Save workflow
  - ▶ Execute: Run workflow with real data
  - 🧪 Test: Run with test/sample data
  - 📊 Analytics: View workflow performance metrics
  - ⚙ Settings: Workflow configuration
  - ↗ Deploy: Publish workflow to production

### 2. Three-Column Layout

#### Left Column: Nodes Panel (~12% width)
- **Node Categories** (color-coded):
  - 🔵 Trigger: Webhook, Schedule, Event listeners
  - 🟢 Action: Execute tasks, call APIs
  - 🟡 Logic: If/Else, Switch, Loop
  - 🟣 Data: Transform, Filter, Merge
  - 🔴 AI/LLM: OpenAI, Claude, Custom models
  - ⚙ Config: Variables, Credentials
- **Drag & Drop**: Drag nodes onto canvas

#### Center Column: Canvas/Workflow Builder (~63% width)
- **Visual Flow Diagram**:
  - Nodes connected by arrows
  - Shows data flow direction
  - Zoom controls (fit to screen, zoom in/out)
  - Grid background for alignment
- **Node Types in Example**:
  1. **Trigger**: Webhook endpoint (/support)
  2. **AI Node**: OpenAI GPT-4 for understanding query
  3. **Condition**: Route based on priority
  4. **High Priority**: Email to human agent
  5. **Low Priority**: Send Slack message
- **Canvas Controls**:
  - Click node to configure
  - Click connection to add intermediate node
  - Right-click for context menu
  - Drag canvas to pan

#### Right Column: Tool Catalogue Panel (~25% width)
- **Search bar** for quick discovery
- **Categorized Items**:
  - Nodes (156): All available node types
  - Agent Library (89): Pre-built agent templates
  - Connectors (78): Integration modules
- **Quick Actions**:
  - Add Node: Insert at cursor position
  - Templates: Load workflow templates
  - Favorites: Quick access to common nodes
  - My Nodes: Custom-built nodes

### 3. Bottom Panel: Execution Log
- Shows real-time execution progress
- Displays errors and warnings
- Links to detailed execution history
- Collapsible to maximize canvas space

---

## Node Configuration Modal

When user clicks on a node:

```
┌───────────────────────────────────────────────────────────┐
│  Configure: OpenAI GPT-4 Node                       [✕]  │
├───────────────────────────────────────────────────────────┤
│                                                           │
│  Node Name:  [AI Node                            ]       │
│                                                           │
│  Model:      [GPT-4 ▼]  [o1-preview] [Claude 3.5]       │
│                                                           │
│  Prompt:                                                  │
│  ┌───────────────────────────────────────────────────┐   │
│  │ Analyze the following customer support request   │   │
│  │ and determine if it requires immediate attention. │   │
│  │                                                   │   │
│  │ Request: {{$node.Webhook.json.message}}          │   │
│  │                                                   │   │
│  │ Classify as: HIGH, MEDIUM, or LOW priority       │   │
│  └───────────────────────────────────────────────────┘   │
│                                                           │
│  Temperature:  [0.7          ] (0-1)                     │
│                                                           │
│  Max Tokens:   [500          ]                           │
│                                                           │
│  Output Format: [JSON ▼]  [Text] [Structured]           │
│                                                           │
│  Advanced Settings ▼                                      │
│  ┌───────────────────────────────────────────────────┐   │
│  │ ☑ Retry on failure (max 3 attempts)              │   │
│  │ ☑ Cache responses (24 hours)                     │   │
│  │ ☐ Log full request/response                      │   │
│  └───────────────────────────────────────────────────┘   │
│                                                           │
│  [Test Node]  [View Docs]                                │
│                                                           │
│              [Cancel]           [Save & Close]            │
│                                                           │
└───────────────────────────────────────────────────────────┘
```

---

## Tool Catalogue Panel - Expanded

```
┌──────────────────────────┐
│  TOOL CATALOGUE         │
│  ─────────────────      │
│                         │
│  🔍 Search nodes...     │
│  ─────────────────      │
│                         │
│  📦 Nodes (156) [▼]     │
│  ├─ 🔵 Triggers (12)    │
│  │   ├─ Webhook         │ ← Drag to canvas
│  │   ├─ Schedule        │
│  │   ├─ Email Watch     │
│  │   └─ File Watch      │
│  ├─ 🔴 AI/LLM (34)      │
│  │   ├─ OpenAI          │
│  │   ├─ Anthropic       │
│  │   ├─ Cohere          │
│  │   └─ Custom Model    │
│  ├─ 🟢 Actions (45)     │
│  ├─ 🟡 Logic (18)       │
│  └─ 🟣 Data (23)        │
│                         │
│  🤖 Agent Library [▶]   │
│                         │
│  🔌 Connectors [▶]      │
│                         │
│  ─────────────────      │
│                         │
│  [View Full Catalogue]  │
│                         │
│  QUICK ACTIONS          │
│  ─────────────────      │
│                         │
│  [+ Add Node]           │
│  [📋 Templates]         │
│  [⭐ Favorites]         │
│  [📦 My Nodes]          │
│                         │
│  WORKFLOW INFO          │
│  ─────────────────      │
│                         │
│  Nodes: 6               │
│  Connections: 6         │
│  Status: Draft          │
│  Last run: Never        │
│  Executions: 0          │
│                         │
└──────────────────────────┘
```

---

## Workflow Templates Gallery

Click "Templates" to see pre-built workflows:

```
┌─────────────────────────────────────────────────────────────┐
│  Workflow Templates                                   [✕]  │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  Popular Templates:                                         │
│                                                             │
│  ┌────────────────┐  ┌────────────────┐  ┌──────────────┐  │
│  │ Customer       │  │ Data Pipeline  │  │ Slack Bot    │  │
│  │ Support Bot    │  │ ETL            │  │              │  │
│  │                │  │                │  │              │  │
│  │ [Preview]      │  │ [Preview]      │  │ [Preview]    │  │
│  │ [Use Template] │  │ [Use Template] │  │ [Use Temp.]  │  │
│  └────────────────┘  └────────────────┘  └──────────────┘  │
│                                                             │
│  Categories:                                                │
│  [All] [AI/ML] [Integration] [Automation] [Analytics]      │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## Execution View (After Running Workflow)

```
┌────────────────────────────────────────────────────────────┐
│  📊 EXECUTION LOG                              [Expand ▲] │
│  ────────────────────────────────────────────────────────  │
│                                                            │
│  Execution #1 - Started: 2:45 PM - Duration: 1.2s        │
│                                                            │
│  ✓ Webhook (0.05s) - Received request                    │
│  ✓ AI Node (0.89s) - Classification: HIGH                │
│  ✓ Condition (0.02s) - Routed to HIGH branch             │
│  ✓ Email Node (0.24s) - Email sent to agent@company.com  │
│                                                            │
│  Status: ✓ Success                                        │
│  [View Full Log] [Export Data] [Debug]                    │
│                                                            │
└────────────────────────────────────────────────────────────┘
```

---

## User Interactions

### 1. Building Workflows
- **Drag Node**: From left panel to canvas
- **Connect Nodes**: Click output port → drag → click input port
- **Configure Node**: Click node → opens configuration modal
- **Delete Node/Connection**: Select and press Delete or right-click
- **Arrange Nodes**: Drag to reposition, auto-layout option available

### 2. Tool Catalogue Integration
- **Search**: Filter nodes by keyword
- **Drag to Canvas**: Direct insertion from catalogue
- **Click Item**: View details and documentation
- **Add to Favorites**: Quick access to frequently used nodes
- **Templates**: Load pre-built workflow patterns

### 3. Testing & Execution
- **Test Mode**: Run with sample data without side effects
- **Execute**: Run with real data in production
- **Debug**: Step through execution node by node
- **Analytics**: View metrics (success rate, avg duration, errors)

### 4. Deployment
- **Save**: Store workflow as draft
- **Deploy**: Publish to production (enables trigger)
- **Version Control**: Track changes, rollback if needed
- **Share**: Collaborate with team members

---

## Navigation Flow

```
Main Dashboard (Screen 03)
    ↓
[User clicks "Low-Code Studio"]
    ↓
Low-Code Studio (THIS SCREEN)
    │
    ├─ [New Workflow] ──► Blank canvas
    ├─ [Templates] ──► Template gallery
    ├─ [My Workflows] ──► Saved workflows list
    │
    └─ [Studios ▼] ──► Switch studio ──► Screen 04/06/07
```

---

## Design Notes

- **Visual Programming**: No coding required, drag-and-drop interface
- **n8n-Inspired**: Familiar to users of visual automation tools
- **Real-time Validation**: Show errors immediately (e.g., missing connections)
- **Auto-save**: Periodic saving every 30 seconds
- **Collaboration**: Show who else is editing (future enhancement)
- **Version History**: Track changes, compare versions
- **Export/Import**: Share workflows as JSON files
- **Extensibility**: Users can create custom nodes
- **Performance**: Handle complex workflows (100+ nodes)
- **Accessibility**: Keyboard shortcuts for power users
- **Mobile View**: Read-only view on mobile, edit on desktop only
