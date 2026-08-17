# CopilotStudio

Microsoft Copilot Studio architecture notes and enterprise chatbot use cases, with annotated screenshots.

![Type](https://img.shields.io/badge/type-documentation-lightgrey?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/vinaygangidi/CopilotStudio?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

## What This Does

Two written walkthroughs of Microsoft Copilot Studio, covering how custom enterprise
chatbots are architected and how conversational topics drive their behavior. Both are
illustrated with annotated screenshots of the Copilot Studio interface.

This is a documentation repository — no code, no bot solution files, no deployable
artifacts.

## How It Works

Nothing executes. The repository holds two article files and fourteen supporting images.

### [Copilot Studio: Your AI Assistant Hub](./Copilot%20Studio%3A%20Your%20AI%20Assistant%20Hub)

Architecture overview:

- What a copilot is, and when to use generative AI versus traditional NLP models from Azure
  Language Services
- Deployment channels — Microsoft Teams, Slack, Skype, customer websites
- Enterprise integration targets — Dynamics 365, Salesforce, ServiceNow — including handoff
  to live agents or other copilots
- The plugin architecture and its four plugin types: Conversational, Flow, Prompt, and
  Connector

### [Copilot Studio AI Assistant: Conversational Topics](./Copilot%20Studio%20AI%20Assistant%20%3A%20Conversational%20Topics)

How topics work:

- Topics as structured conversation paths that absorb varied phrasings of the same intent
  ("Can you book a meeting?" and "I need to set up a call" both routing to *Schedule a
  Meeting*)
- Custom topics versus system topics, and why system topics cannot be deleted
- Trigger phrases and unknown-intent handling
- Local and global variables for storing user responses and intents
- The topics canvas and its available connectors

### Screenshots

Fourteen images support the articles: `Architecture.png`, `Studio1`–`Studio6`,
`Topics.JPG`, `TopicManagementConnectors.JPG`, `TriggerPhrases.JPG`,
`TriggerPhrases1.JPG`, `ActionConnectors.JPG`, `AdvancedConnectors.JPG`,
`MultipleConnectors.JPG`, and `code-editor-conversation.png`.

## Quickstart

There is nothing to install or run.

1. Clone or browse the repository:
   ```bash
   git clone https://github.com/vinaygangidi/CopilotStudio.git
   cd CopilotStudio
   ```

2. Read the two article files. Both are plain text with inline image references and render
   on GitHub.

3. To follow along in the product, sign in to [Copilot Studio](https://copilotstudio.microsoft.com)
   with a Microsoft 365 or Power Platform license.

## Configuration

Not applicable. No code, dependencies, or environment variables.

| Item | Notes |
|---|---|
| Articles | 2 plain-text files, no extension |
| Images | 14 files (`.JPG`, `.jpg`, `.png`) |
| License | MIT |

## Limitations

- **Documentation only.** No bot solution files, no Power Platform export, no code. Nothing
  here can be imported into Copilot Studio.
- **Written in 2024 against a moving product.** Copilot Studio has been renamed and
  restructured repeatedly since these were written. The plugin taxonomy, canvas layout, and
  screenshots no longer match the current interface, and Microsoft has since folded much of
  this into agent-centric terminology.
- **Screenshots will keep drifting.** Every image captures a UI that has already changed.
- **Article files have no extension.** Neither is named `.md`, so GitHub renders them as
  plain text without formatting, and one contains a colon in its filename, which complicates
  linking and can break checkouts on some Windows configurations.
- **Images are hosted inline via `user-attachments` URLs.** The articles reference GitHub
  attachment URLs rather than the committed image files, so the rendered articles depend on
  GitHub's attachment service remaining available even though local copies exist.
- **No verification of product claims.** Integration and channel capabilities are described
  as of writing and were not re-checked against current Microsoft documentation.
- **Not a tutorial.** The articles explain concepts but contain no step-by-step build,
  exercise, or sample bot to reproduce.

## License

MIT — see [LICENSE](LICENSE).
