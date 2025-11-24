# Main Dashboard - Unified Hub

## Screen Purpose
Central hub that appears after workspace provisioning. Allows users to switch between different studios, access shared resources, and manage their workspace.

---

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│  AI AGENTIC PLATFORM                                     [User: John]  [Settings] ⚙ │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                      │
│  Home > My Workspace                                                                 │
│                                                                                      │
│  ┌────────────────────────────────────────────────────────────────────────────────┐ │
│  │                                                                                 │ │
│  │  👋 Welcome back, John                      Workspace: Low-Code Builder        │ │
│  │                                                                                 │ │
│  │  Quick Actions:                                                                │ │
│  │  [📊 Switch Studio]  [📁 My Projects]  [🔍 Browse Catalogue]  [📚 Resources]  │ │
│  │                                                                                 │ │
│  └────────────────────────────────────────────────────────────────────────────────┘ │
│                                                                                      │
│                                                                                      │
│  STUDIO ENVIRONMENTS                                                                 │
│  ───────────────────────────────────────────────────────────────────────────────    │
│                                                                                      │
│  ┌──────────────────────┐  ┌──────────────────────┐  ┌──────────────────────┐     │
│  │ 🔧 LOW-CODE STUDIO  │  │ 📊 DATA SCIENCE     │  │ 📝 DECLARATIVE      │     │
│  │    (ACTIVE)          │  │    STUDIO           │  │    BUILDER          │     │
│  │ ──────────────────   │  │ ──────────────────  │  │ ──────────────────  │     │
│  │                      │  │                     │  │                     │     │
│  │ Visual workflow      │  │ Notebooks & ML      │  │ Form-based agent    │     │
│  │ builder with n8n     │  │ model training      │  │ configuration       │     │
│  │                      │  │                     │  │                     │     │
│  │ Last used: Now       │  │ Last used: Never    │  │ Last used: 2d ago   │     │
│  │                      │  │                     │  │                     │     │
│  │ [Continue Working]   │  │ [Launch Studio]     │  │ [Launch Studio]     │     │
│  │                      │  │                     │  │                     │     │
│  └──────────────────────┘  └──────────────────────┘  └──────────────────────┘     │
│                                                                                      │
│  ┌──────────────────────┐                                                           │
│  │ 📈 BUSINESS          │                                                           │
│  │    ANALYTICS         │                                                           │
│  │ ──────────────────   │                                                           │
│  │                      │                                                           │
│  │ Reports & dashboards │                                                           │
│  │                      │                                                           │
│  │ Last used: 1w ago    │                                                           │
│  │                      │                                                           │
│  │ [Launch Studio]      │                                                           │
│  │                      │                                                           │
│  └──────────────────────┘                                                           │
│                                                                                      │
│                                                                                      │
│  RECENT ACTIVITY                                      SHARED RESOURCES               │
│  ───────────────────                                  ─────────────────              │
│                                                                                      │
│  📄 Customer Support Bot                              🔧 Tool Catalogue (245)        │
│     Modified 2 hours ago                              🤖 Agent Templates (89)        │
│     Declarative Builder                               🔌 Integrations (156)          │
│                                                       📖 Documentation                │
│  🔄 Data Pipeline v2.1                                💬 Community Forum             │
│     Modified Yesterday                                                               │
│     Low-Code Studio                                   [Browse All →]                 │
│                                                                                      │
│  📊 Sales Analytics Dashboard                                                        │
│     Modified 3 days ago                                                              │
│     Business Analytics                                                               │
│                                                                                      │
│  [View All Projects →]                                                               │
│                                                                                      │
│                                                                                      │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Key Components

### 1. Header Bar
- Platform branding
- Breadcrumb navigation (Home > My Workspace)
- User profile + Settings

### 2. Welcome Section
- Personalized greeting
- Current workspace context
- Quick action buttons

### 3. Studio Environments Grid
- Shows ALL available studios regardless of initial persona selection
- **Active Studio**: Highlighted with special indicator
- **Never Used**: Show "Launch Studio" instead of "Continue Working"
- Each card shows:
  - Studio name and icon
  - Brief description
  - Last used timestamp
  - Primary CTA button

### 4. Recent Activity Panel (Left)
- Recently modified projects across all studios
- Shows which studio was used for each project
- Quick access to continue work

### 5. Shared Resources Panel (Right)
- Links to platform-wide features:
  - Tool Catalogue (with count)
  - Agent Templates (with count)
  - Integrations (with count)
  - Documentation
  - Community Forum

---

## Studio Cards - Detailed Breakdown

### Low-Code Studio (Active)
```
┌──────────────────────┐
│ 🔧 LOW-CODE STUDIO  │ ← Icon + Title
│    (ACTIVE) ★       │ ← Status badge
│ ──────────────────   │
│                      │
│ Visual workflow      │ ← Description
│ builder with n8n     │
│                      │
│ Last used: Now       │ ← Usage info
│ 3 active workflows   │ ← Context data
│                      │
│ [Continue Working]   │ ← Primary CTA
│  View Projects       │ ← Secondary action
│                      │
└──────────────────────┘
```

### Data Science Studio (Not Yet Used)
```
┌──────────────────────┐
│ 📊 DATA SCIENCE     │
│    STUDIO            │
│ ──────────────────   │
│                      │
│ Notebooks & ML       │
│ model training       │
│                      │
│ Last used: Never     │
│ 0 notebooks          │
│                      │
│ [Launch Studio]      │ ← First time launch
│  View Tutorial       │
│                      │
└──────────────────────┘
```

---

## User Interactions

### 1. Quick Actions
- **Switch Studio**: Opens studio selection modal/dropdown
- **My Projects**: Filtered view of all projects across studios
- **Browse Catalogue**: Opens integrated catalogue panel
- **Resources**: Opens documentation/learning center

### 2. Studio Cards
- **Click Card**: Opens full studio environment (Screen 04-07)
- **Hover**: Show additional context (# of projects, resources used)
- **View Projects**: Filtered list of projects for that studio

### 3. Recent Activity
- **Click Project**: Opens project in appropriate studio
- **Right-click**: Context menu (rename, delete, share, etc.)

### 4. Shared Resources
- **Browse All**: Opens full catalogue view with filters
- **Click Individual Resource**: Deep link to specific section

---

## Navigation Flow

```
Workspace Provisioning (Screen 02)
    ↓ (automatic)
Main Dashboard (THIS SCREEN)
    ↓
[User selects a studio]
    ↓
Specific Studio Environment (Screen 04-07)
    ↓
[User can return to Dashboard via breadcrumb/menu]
    ↓
Main Dashboard (THIS SCREEN)
```

---

## Switching Studios - Modal Example

When user clicks "Switch Studio" or a studio card:

```
┌─────────────────────────────────────────────┐
│  Switch to Different Studio          [✕]   │
├─────────────────────────────────────────────┤
│                                             │
│  Select the studio you want to work in:    │
│                                             │
│  ○ Low-Code Studio (Currently Active)      │
│  ○ Data Science Studio                     │
│  ○ Declarative Builder                     │
│  ○ Business Analytics                      │
│                                             │
│  ☑ Save my current work before switching   │
│                                             │
│           [Cancel]      [Switch Studio]     │
│                                             │
└─────────────────────────────────────────────┘
```

---

## Mobile/Responsive Behavior

- Studio cards stack vertically on smaller screens
- Recent Activity and Shared Resources stack below studios
- Quick Actions become hamburger menu
- Prioritize active studio at top

---

## Design Notes

- **Unified Experience**: All studios accessible from one hub
- **Context Preservation**: Each studio maintains independent state
- **Discoverability**: Users can explore all capabilities, not locked into persona
- **Breadcrumbs**: Always provide path back to dashboard
- **State Indication**: Clear visual indicator of which studio is "active"
- **Onboarding**: First-time users see tutorial prompts for unused studios
- **Resource Limits**: Show quota/usage if applicable (e.g., "2/5 active studios")
- **Collaboration**: Future enhancement - show collaborators working in shared workspace
