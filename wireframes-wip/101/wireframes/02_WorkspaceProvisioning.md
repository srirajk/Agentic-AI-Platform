# Workspace Provisioning

## Screen Purpose
Loading/transition state shown while the platform provisions an isolated workspace environment for the selected persona.

---

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│  AI AGENTIC PLATFORM                                     [User: John]  [Settings] ⚙ │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                          🔧  Setting Up Your Workspace                               │
│                                                                                      │
│                                                                                      │
│                           Profile: Low-Code Builder                                  │
│                                                                                      │
│                                                                                      │
│                    ┌─────────────────────────────────────┐                          │
│                    │  ████████████████░░░░░░░░░░░  75%   │                          │
│                    └─────────────────────────────────────┘                          │
│                                                                                      │
│                                                                                      │
│                         Provisioning Resources:                                      │
│                                                                                      │
│                         ✓  Initializing workspace container                         │
│                         ✓  Loading studio environment                               │
│                         ✓  Connecting to tool registry                              │
│                         ⟳  Configuring integrations...                              │
│                         ○  Preparing agent catalogue                                │
│                         ○  Setting up collaboration features                        │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                    Estimated time remaining: ~15 seconds                             │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                           [ Cancel and Return ]                                      │
│                                                                                      │
│                                                                                      │
│                                                                                      │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Alternative State: Quick Launch (Existing Workspace)

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│  AI AGENTIC PLATFORM                                     [User: John]  [Settings] ⚙ │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                          ⚡ Launching Your Workspace                                 │
│                                                                                      │
│                                                                                      │
│                           Profile: Data Scientist                                    │
│                      Workspace: ML Pipeline Project                                  │
│                                                                                      │
│                                                                                      │
│                    ┌─────────────────────────────────────┐                          │
│                    │  ████████████████████████████  90%  │                          │
│                    └─────────────────────────────────────┘                          │
│                                                                                      │
│                                                                                      │
│                         Restoring Session:                                           │
│                                                                                      │
│                         ✓  Loading workspace state                                  │
│                         ✓  Reconnecting to resources                                │
│                         ⟳  Restoring notebooks and files...                         │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                                                                                      │
│                                                                                      │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Provisioning Steps (Backend Process)

### New Workspace Creation

1. **✓ Initializing workspace container**
   - Spin up isolated environment (container/VM)
   - Allocate compute resources
   - Duration: ~3-5 seconds

2. **✓ Loading studio environment**
   - Install studio-specific dependencies
   - Configure IDE/interface components
   - Duration: ~5-7 seconds

3. **✓ Connecting to tool registry**
   - Establish connection to central tool/agent catalogue
   - Load available integrations
   - Duration: ~2-3 seconds

4. **⟳ Configuring integrations** (Currently Processing)
   - Set up pre-configured connectors
   - Initialize API connections
   - Duration: ~4-6 seconds

5. **○ Preparing agent catalogue** (Pending)
   - Load persona-specific agent templates
   - Sync custom agents
   - Duration: ~2-3 seconds

6. **○ Setting up collaboration features** (Pending)
   - Enable sharing/collaboration tools
   - Configure workspace permissions
   - Duration: ~2-3 seconds

### Existing Workspace Resume

- Faster loading (~5-10 seconds total)
- Restores previous session state
- Reconnects to existing resources

---

## Status Indicators

- **✓** Completed step (green/success)
- **⟳** In progress (blue/spinning animation)
- **○** Pending (gray/waiting)
- **✗** Failed (red - triggers error state)

---

## Error State Example

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                      │
│                          ⚠️  Workspace Provisioning Failed                           │
│                                                                                      │
│                                                                                      │
│                  Unable to connect to tool registry                                  │
│                  Error Code: CONN_TIMEOUT_503                                        │
│                                                                                      │
│                                                                                      │
│                         [Retry Provisioning]    [Report Issue]                      │
│                                                                                      │
│                              [Return to Home]                                        │
│                                                                                      │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

---

## User Interactions

1. **Automatic**: Screen appears immediately after profile selection
2. **Progress Updates**: Real-time status updates every 1-2 seconds
3. **Cancel Option**: Allows user to abort and return to profile selection
4. **Error Handling**: Clear error messages with retry/support options
5. **Completion**: Auto-transitions to Main Dashboard (Screen 03) upon 100% completion

---

## Navigation Flow

```
Profile Selection (Screen 01)
    ↓
[User clicks "Launch Studio"]
    ↓
Workspace Provisioning (THIS SCREEN)
    ↓ (automatic on completion)
Main Dashboard (Screen 03)
```

---

## Design Notes

- **Animation**: Smooth progress bar animation, spinner on active step
- **Transparency**: Show what's happening "under the hood" to build trust
- **Time Estimates**: Helps manage user expectations
- **Optimistic Loading**: Pre-load static assets while provisioning
- **Timeout Handling**: Maximum wait time of 60 seconds before error state
- **Logging**: All steps logged for debugging/support purposes
- **Performance Metrics**: Track provisioning time for optimization
