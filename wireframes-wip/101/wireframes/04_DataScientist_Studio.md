# Data Scientist Studio

## Screen Purpose
SageMaker-style environment for ML/AI development, model training, and experimentation with Jupyter notebooks.

---

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
│  AI AGENTIC PLATFORM                                                     [User: John]  [Settings] ⚙        │
├─────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
│  Home > My Workspace > Data Science Studio                                                                  │
│                                                                                                              │
│  ┌────────────────────────────────────────────────────────────────────────────────────────┐                 │
│  │  📊 DATA SCIENCE STUDIO               [≡ Studios ▼] [💾 Save] [▶ Run] [⏹ Stop]       │                 │
│  └────────────────────────────────────────────────────────────────────────────────────────┘                 │
│                                                                                                              │
│  ┌──────┬─────────────────────────────────────────────────────────────────────┬───────────────────────────┐ │
│  │ FILE │                    MAIN WORKSPACE                                    │  TOOL CATALOGUE          │ │
│  │ NAV  │                                                                      │  ─────────────────       │ │
│  ├──────┤                                                                      │                          │ │
│  │      │  ┌──────────────────────────────────────────────────────────────┐   │  🔍 Search tools...      │ │
│  │ 📁   │  │  Notebook: customer_churn_model.ipynb            [Cell ▼]  │   │  ─────────────────       │ │
│  │ Pro  │  ├──────────────────────────────────────────────────────────────┤   │                          │ │
│  │ ject │  │  # Customer Churn Prediction Model                          │   │  📦 ML Models (45)       │ │
│  │ s    │  │                                                              │   │  ├─ Transformers         │ │
│  │      │  │  import pandas as pd                                        │   │  ├─ Scikit-learn         │ │
│  │ • ML │  │  import numpy as np                                         │   │  ├─ PyTorch               │ │
│  │   Pi │  │  from sklearn.ensemble import RandomForestClassifier       │   │  └─ TensorFlow            │ │
│  │   pe │  │                                                              │   │                          │ │
│  │   li │  │  # Load data                                                │   │  🔧 Data Tools (23)      │ │
│  │   ne │  │  df = pd.read_csv('customer_data.csv')                     │   │  ├─ Pandas               │ │
│  │      │  │  df.head()                                                  │   │  ├─ NumPy                │ │
│  │ • Cu │  │                                                              │   │  ├─ SQL Connectors       │ │
│  │   st │  │  [▶ Run Cell]  [+ Code]  [+ Markdown]                       │   │  └─ Data Validators      │ │
│  │   om │  └──────────────────────────────────────────────────────────────┘   │                          │ │
│  │   er │                                                                      │  🤖 Agent Tools (67)     │ │
│  │   Ch │  Output:                                                             │  ├─ LangChain            │ │
│  │   ur │  ┌──────────────────────────────────────────────────────────────┐   │  ├─ AutoGen              │ │
│  │   n  │  │  CustomerID  Age  Tenure  MonthlyCharges  Churn             │   │  ├─ CrewAI               │ │
│  │      │  │  ────────────────────────────────────────────────────────   │   │  └─ Custom Agents        │ │
│  │ 📁   │  │  1001       34   12      89.99           No                 │   │                          │ │
│  │ Not  │  │  1002       45   24      120.50          Yes                │   │  🔌 Integrations (34)    │ │
│  │ ebo  │  │  1003       28   6       65.00           No                 │   │  ├─ AWS Services         │ │
│  │ oks  │  │  1004       52   48      150.25          No                 │   │  ├─ Databases            │ │
│  │      │  │  1005       39   18      95.75           Yes                │   │  ├─ APIs                 │ │
│  │ • ch │  └──────────────────────────────────────────────────────────────┘   │  └─ Cloud Storage        │ │
│  │   ur │                                                                      │                          │ │
│  │   n. │  ┌──────────────────────────────────────────────────────────────┐   │  ─────────────────       │ │
│  │   ip │  │  # Feature Engineering                                       │   │                          │ │
│  │   yn │  │  df['tenure_age_ratio'] = df['Tenure'] / df['Age']         │   │  [View Full Catalogue]   │ │
│  │   b  │  │                                                              │   │                          │ │
│  │      │  │  # Train model                                               │   │  QUICK ACTIONS           │ │
│  │ • ex │  │  model = RandomForestClassifier()                           │   │  ─────────────────       │ │
│  │   plo│  │  model.fit(X_train, y_train)                                │   │                          │ │
│  │   re │  │                                                              │   │  [+ Import Tool]         │ │
│  │   .i │  │  [▶ Run Cell]  [+ Code]  [+ Markdown]                       │   │  [⭐ View Favorites]     │ │
│  │   py │  └──────────────────────────────────────────────────────────────┘   │  [📊 My Custom Tools]    │ │
│  │   nb │                                                                      │                          │ │
│  │      │                                                                      │                          │ │
│  │ 📁   │                                                                      │                          │ │
│  │ Dat  │                                                                      │                          │ │
│  │ a    │                                                                      │                          │ │
│  │      │                                                                      │                          │ │
│  │ 📁   │                                                                      │                          │ │
│  │ Mod  │                                                                      │                          │ │
│  │ els  │                                                                      │                          │ │
│  │      │                                                                      │                          │ │
│  └──────┴──────────────────────────────────────────────────────────────────────┴──────────────────────────┘ │
│                                                                                                              │
│  ┌────────────────────────────────────────────────────────────────────────────────────────────────────────┐ │
│  │  COMPUTE RESOURCES                      EXPERIMENTS                       JOBS                         │ │
│  │  ────────────────────                   ───────────                       ────                         │ │
│  │  Instance: ml.t3.medium (Running)       churn_model_v1 (Active)          3 completed, 0 running       │ │
│  │  CPU: 45% | Memory: 2.1GB/4GB           Accuracy: 0.87                   [View All Jobs]              │ │
│  │  [Scale Up]  [Stop Instance]            [View Metrics]                                                │ │
│  └────────────────────────────────────────────────────────────────────────────────────────────────────────┘ │
│                                                                                                              │
└─────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Key Components

### 1. Studio Header
- Studio name and icon (📊 Data Science Studio)
- **Studios Dropdown**: Quick switch to other studios
- **Save Button**: Save current notebook/code
- **Run/Stop Controls**: Execute cells or training jobs

### 2. Three-Column Layout

#### Left Column: File Navigator (~15% width)
- Project folders structure
- Notebooks (.ipynb files)
- Data files
- Model files
- Collapsible for more workspace

#### Center Column: Main Workspace (~60% width)
- **Notebook Interface** (Jupyter-style)
  - Code cells with syntax highlighting
  - Output cells showing results (tables, charts, logs)
  - Cell controls (Run, Add Code/Markdown)
  - Multiple tabs for multiple notebooks
- **Alternative Views**:
  - Model training interface
  - Dataset explorer
  - Experiment dashboard

#### Right Column: Tool Catalogue Panel (~25% width)
- **Search bar** for quick tool discovery
- **Categorized tools**:
  - ML Models (transformers, sklearn, pytorch, etc.)
  - Data Tools (pandas, numpy, connectors)
  - Agent Tools (LangChain, AutoGen, CrewAI)
  - Integrations (AWS, databases, APIs)
- **Expandable categories** with item counts
- **Quick actions**:
  - Import tool (installs dependencies)
  - View favorites
  - My custom tools

### 3. Bottom Status Bar
- **Compute Resources**:
  - Current instance type
  - CPU/Memory usage
  - Scale up/down controls
- **Experiments**:
  - Active experiment tracking
  - Current metrics (accuracy, loss, etc.)
  - Link to detailed metrics dashboard
- **Jobs**:
  - Training job status
  - Job history

---

## Tool Catalogue Panel - Expanded View

```
┌───────────────────────────┐
│  TOOL CATALOGUE          │
│  ─────────────────       │
│                          │
│  🔍 Search tools...      │
│  ─────────────────       │
│                          │
│  📦 ML Models (45) [▼]   │
│  ├─ 🤗 Transformers      │
│  │   ├─ BERT            │ ← Click to see details
│  │   ├─ GPT-2           │
│  │   └─ T5              │
│  ├─ Scikit-learn        │
│  ├─ PyTorch             │
│  └─ TensorFlow          │
│                          │
│  🔧 Data Tools (23) [▶]  │
│                          │
│  🤖 Agent Tools (67) [▶] │
│                          │
│  🔌 Integrations (34)[▶] │
│                          │
│  ─────────────────       │
│                          │
│  [View Full Catalogue]   │
│                          │
│  QUICK ACTIONS           │
│  ─────────────────       │
│                          │
│  [+ Import Tool]         │
│  [⭐ View Favorites]     │
│  [📊 My Custom Tools]    │
│                          │
└───────────────────────────┘
```

### Tool Detail Modal (Click on Tool)

```
┌───────────────────────────────────────────────────┐
│  BERT - Transformer Model                   [✕]  │
├───────────────────────────────────────────────────┤
│                                                   │
│  📦 transformers.BertModel                        │
│  Version: 4.35.0                                  │
│                                                   │
│  Description:                                     │
│  Bidirectional Encoder Representations from      │
│  Transformers for NLP tasks                      │
│                                                   │
│  Installation:                                    │
│  pip install transformers                         │
│                                                   │
│  Quick Start:                                     │
│  ┌─────────────────────────────────────────────┐ │
│  │  from transformers import BertModel         │ │
│  │  model = BertModel.from_pretrained('bert')  │ │
│  │  # Use model for your task                  │ │
│  └─────────────────────────────────────────────┘ │
│                                                   │
│  [Insert Code Snippet]  [View Documentation]     │
│  [⭐ Add to Favorites]  [Install Package]         │
│                                                   │
└───────────────────────────────────────────────────┘
```

---

## User Interactions

### 1. Working with Notebooks
- **Run Cell**: Execute current cell (Shift+Enter)
- **Add Cell**: Insert new code or markdown cell
- **Cell Output**: Displays results (text, tables, visualizations)
- **Multiple Tabs**: Work on multiple notebooks simultaneously

### 2. Tool Catalogue Integration
- **Drag & Drop**: Drag tool from catalogue into code cell
- **Click Tool**: Opens detail modal with documentation
- **Insert Code**: Automatically adds import/usage code to active cell
- **Install Package**: One-click dependency installation
- **Search**: Real-time filtering of tools
- **Favorites**: Quick access to frequently used tools

### 3. Resource Management
- **Monitor Usage**: Real-time CPU/memory tracking
- **Scale Instance**: Upgrade compute resources for heavy training
- **Stop Instance**: Save costs when not in use

### 4. Experiment Tracking
- **Automatic Logging**: Tracks metrics from training runs
- **View Metrics**: Detailed charts and comparison dashboard
- **Version Control**: Compare different model versions

---

## Alternative View: Model Training Dashboard

```
┌──────────────────────────────────────────────────────────────────┐
│  TRAINING DASHBOARD                                              │
├──────────────────────────────────────────────────────────────────┤
│                                                                  │
│  Model: customer_churn_rf_v2                                    │
│  Status: ████████████████░░░░ 78% (Epoch 78/100)               │
│                                                                  │
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────┐  │
│  │  Training Loss   │  │  Validation Acc  │  │  Time/Epoch  │  │
│  │                  │  │                  │  │              │  │
│  │    0.234         │  │     0.874        │  │   1.2s       │  │
│  │    ↓ -12%       │  │     ↑ +3%       │  │              │  │
│  └──────────────────┘  └──────────────────┘  └──────────────┘  │
│                                                                  │
│  [Chart: Loss curve over epochs]                                │
│  [Chart: Accuracy curve over epochs]                            │
│                                                                  │
│  [⏸ Pause]  [⏹ Stop]  [💾 Save Checkpoint]                     │
│                                                                  │
└──────────────────────────────────────────────────────────────────┘
```

---

## Navigation Flow

```
Main Dashboard (Screen 03)
    ↓
[User clicks "Data Science Studio"]
    ↓
Data Science Studio (THIS SCREEN)
    │
    ├─ [Notebooks] ──► Jupyter interface
    ├─ [Model Training] ──► Training dashboard
    ├─ [Experiments] ──► Experiment tracking
    ├─ [Data] ──► Dataset explorer
    │
    └─ [Studios ▼] ──► Switch to other studio ──► Screen 05/06/07
```

---

## Design Notes

- **Jupyter Compatibility**: Familiar interface for data scientists
- **Integrated Tooling**: No need to leave platform to find packages
- **Resource Visibility**: Always show compute usage to manage costs
- **Experiment Tracking**: Built-in MLOps capabilities
- **Collaboration**: Share notebooks with team (future enhancement)
- **Version Control**: Git integration for code versioning
- **Cloud Integration**: Direct connection to AWS SageMaker, S3, etc.
- **Keyboard Shortcuts**: Support standard Jupyter shortcuts
- **Auto-save**: Periodic saving to prevent data loss
- **Export Options**: Download notebooks as .ipynb, .py, or HTML
