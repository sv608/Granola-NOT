# Agent for DevOps — capabilities, creation, and landing page strategy

- **Date:** Aug 13, 2026 8:59 PM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/5fe7a249-4c65-4e32-a234-5102a7a4970f
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

# Agent for DevOps: Core Capabilities

- Covers the full dev lifecycle: requirement gathering, code quality, test case creation, bug/vulnerability detection, compliance checking
- Triggered manually, on a schedule, or via events (pull request, pipeline, work item creation, build/release)
- Human-in-the-loop built into most agents: AI generates a draft, human reviews and approves before merge
- Agents run concurrently/in parallel
- Versioning supported: full history of agent instruction changes, reviewable per version

# Agent Types

- Autonomous agents: invoke LLM, generate dynamic results, handle complex reasoning tasks
  - Examples: BA requirement analysis, QA test case generation, DevOps pipeline checks, Release Manager compliance review
- Execution agents: no LLM at runtime, run deterministic logic from pre-generated code
  - Example: risk score calculator using a fixed formula (severity x probability x durability = risk index)
  - Same output every time; suited for repetitive mathematical or rule-based tasks

# Agent Creation and Skills

- Three creation modes:
  1. AI-assisted: provide a short description, AI generates full instructions and agent name
  2. Manual: write instructions in plain English, no code needed
  3. Library template: use a prebuilt agent, modify instructions as needed
- Skills are prebuilt capabilities (e.g., validate acceptance criteria, PR automation, repo operations)
  - Agent auto-selects relevant skills based on relevancy score (shown as %)
  - Custom skills can be created or modified from the skills library
  - Skills function like a runbook: checklist of checks the agent performs (code quality, security, edge cases, etc.)

# Logs, Audit Trail, and Compliance

- Usage logs available at 30, 90, and 120-day ranges
  - Shows credits used per agent, number of runs, timestamps, and model used
  - Filterable by agent name, execution model, credit range, and date range
  - PDF export available
- Per-job logs show full agent output: pull request details, severity, evidence, proposed remediation, test coverage impact
- Copilot for DevOps chat: interact with agents inline, invoke library agents via chat, take actions directly from logs
- Audit trail gap: current logs do not show who triggered an agent or who made changes
  - In-depth audit trail (user-level tracking) is on the roadmap for the next release
- Compliance agents: run against industry-specific standards on a schedule; generate compliance reports

# Landing Page Strategy and Next Steps

- Current draft covers: BA agent workflow, manual vs. agent time comparison, six use cases, two agent types, human-in-the-loop, parallel execution, FAQ
- Gaps identified:
  - Agent types section should precede use cases
  - Missing: regulatory/compliance section, audit trail/export, skills, AI model selection, agent creation flow
  - Industry-specific use case examples needed for credibility
- Agreed approach: live demo session covering BA, QA, and DevOps agents end-to-end, with real execution and compliance examples

# Next Steps

- **Prepare and deliver live demo of Agent for DevOps**

  Cover BA, QA, and DevOps agents: full creation-to-execution flow, human-in-the-loop, skill assignment, audit trail, and compliance standards. Target: this weekend (Friday or Saturday).
- **Prepare doc with 5+ use cases per agent type**

  Include scenario, agent execution steps, and results generated, to feed landing page content and brainstorm further use cases.
