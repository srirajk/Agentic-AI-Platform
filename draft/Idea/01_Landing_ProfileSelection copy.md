# Landing Page - Profile Selection

## Screen Purpose
Entry point where users select their persona/role to access the appropriate studio environment.

---

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│  AI AGENTIC PLATFORM                                     [User: John]  [Settings] ⚙ │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                      │
│                          Welcome to Your AI Workspace                                │
│                        Select your role to get started                               │
│                                                                                      │
│                                                                                      │
│   ┌──────────────────────┐  ┌──────────────────────┐  ┌──────────────────────┐    │
│   │  📊 DATA SCIENTIST   │  │  🔧 LOW-CODE        │  │  📝 DECLARATIVE      │    │
│   │                      │  │     BUILDER         │  │     BUILDER          │    │
│   │  ─────────────────   │  │  ─────────────────  │  │  ─────────────────   │    │
│   │                      │  │                     │  │                      │    │
│   │  Build ML models,    │  │  Create workflows   │  │  Configure agents    │    │
│   │  train agents, and   │  │  visually with      │  │  using forms and     │    │
│   │  experiment with     │  │  drag-and-drop      │  │  templates without   │    │
│   │  notebooks           │  │  nodes              │  │  coding              │    │
│   │                      │  │                     │  │                      │    │
│   │  Tools:              │  │  Tools:             │  │  Tools:              │    │
│   │  • Jupyter           │  │  • n8n Studio       │  │  • Agent Templates   │    │
│   │  • SageMaker         │  │  • Integration Hub  │  │  • Config Builder    │    │
│   │  • Model Training    │  │  • API Connectors   │  │  • Prompt Library    │    │
│   │                      │  │                     │  │                      │    │
│   │  [Launch Studio] ──► │  │  [Launch Studio] ──►│  │  [Launch Studio] ──► │    │
│   │                      │  │                     │  │                      │    │
│   └──────────────────────┘  └──────────────────────┘  └──────────────────────┘    │
│                                                                                      │
│                                                                                      │
│   ┌──────────────────────┐  ┌──────────────────────┐                               │
│   │  📈 BUSINESS         │  │  ➕ CUSTOM ROLE      │                               │
│   │     ANALYST          │  │                      │                               │
│   │  ─────────────────   │  │  ─────────────────   │                               │
│   │                      │  │                      │                               │
│   │  Analyze data,       │  │  Request a custom    │                               │
│   │  create reports,     │  │  studio environment  │                               │
│   │  build dashboards    │  │  for your specific   │                               │
│   │                      │  │  use case            │                               │
│   │  Tools:              │  │                      │                               │
│   │  • Analytics Studio  │  │  Available for:      │                               │
│   │  • Report Builder    │  │  • Enterprise users  │                               │
│   │  • Data Explorer     │  │  • Custom integrations                               │
│   │                      │  │                      │                               │
│   │  [Launch Studio] ──► │  │  [Request Access]    │                               │
│   │                      │  │                      │                               │
│   └──────────────────────┘  └──────────────────────┘                               │
│                                                                                      │
│                                                                                      │
│   Recent Workspaces:                                                                 │
│   • ML Pipeline Project (Data Scientist) - Last accessed: 2 hours ago               │
│   • Customer Support Bot (Declarative Builder) - Last accessed: Yesterday           │
│                                                                                      │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Key Components

### 1. Header
- Platform branding
- User profile indicator
- Settings access

### 2. Profile Cards (Personas)
- **Data Scientist**: ML/AI development focus
- **Low-code Builder**: Visual workflow creation
- **Declarative Builder**: Template-based agent configuration
- **Business Analyst**: Analytics and reporting
- **Custom Role**: Enterprise extensibility option

### 3. Each Card Contains
- Icon/visual identifier
- Role title
- Brief description (value proposition)
- Key tools/capabilities available
- CTA button to launch studio

### 4. Recent Workspaces Section
- Quick access to previously used environments
- Shows role context and last accessed time

---

## User Interactions

1. **Hover State**: Card elevates, shows "Learn More" option
2. **Click "Launch Studio"**:
   - Triggers workspace provisioning (Screen 02)
   - System prepares isolated environment
   - Routes to appropriate studio based on selection
3. **Click Recent Workspace**: Direct access to existing workspace
4. **Multiple selections possible**: Users can have concurrent workspaces

---

## Navigation Flow

```
Landing (Profile Selection)
    ↓
[User selects profile]
    ↓
Workspace Provisioning (Screen 02)
    ↓
Main Dashboard (Screen 03)
    ↓
Specific Studio (Screens 04-07)
```

---

## Design Notes

- **Responsive**: Cards reflow on smaller screens (2x2 grid on mobile)
- **Accessibility**: Keyboard navigation between cards, ARIA labels
- **Visual Hierarchy**: Primary personas (top row) vs secondary options
- **Empty State**: For first-time users, show "Getting Started" tutorial option
- **Workspace Limits**: Display quota if user has workspace limits (e.g., "2/5 active workspaces")
