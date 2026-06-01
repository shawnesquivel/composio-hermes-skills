# OpenAI Academy: Using Skills

*April 10, 2026*  
[OpenAI Academy Skills](https://openai.com/academy/skills/)

---

## Using Skills

Create reusable workflows that guide ChatGPT through recurring tasks.

> **Listen to article**  
> *5:24*

Skills turn the way you already work into reusable workflows that ChatGPT can follow consistently—so you spend less time re-explaining steps, formats, and requirements, and more time getting to a solid result.

If you’ve ever found yourself reusing the same prompt or pasting the same template repeatedly, skills are designed to fix that.

---

## What are Skills?

A **skill** is a reusable, shareable workflow that tells ChatGPT how to perform a specific task. Rather than starting from scratch each time, you define the process once so it can be reliably applied whenever the task comes up.

A skill typically includes:

- **Name and description:** Help ChatGPT recognize when the skill is relevant.
- **Workflow instructions:** Step-by-step guidance for the workflow—usually written in a file called `SKILL.md`.
- **Resources:** Supporting materials the workflow depends on, like templates, examples, brand guidelines, schemas, or tool access.

---

## Why Use Skills?

Skills are most helpful when getting a good output from ChatGPT depends on following a repeatable approach, especially when tasks involve multiple steps, structured formats, or specific requirements.

**Skills help with:**

- **Consistency:** Fewer missed sections, less drift in tone or format, and closer adherence to preferred format.
- **Built-in best practices:** Lightweight enough for everyday users, but grounded in SME-approved workflows.
- **Sharing the playbook:** Teams can use the same standard process directly in ChatGPT instead of relying on informal or undocumented knowledge.
- **Reuse across surfaces:** Build once and apply broadly across different chats and use cases.

---

## What’s a `SKILL.md` File?

A `SKILL.md` file is the skill’s playbook: a plain-text set of instructions that tells ChatGPT how to run a workflow consistently. It’s written in Markdown, a lightweight formatting style that uses simple symbols—like `#` for headings and `-` for lists—so the file is easy to read and edit in most tools.

Because it’s plain text and Markdown-based, `SKILL.md` is portable. It can be shared, versioned, and reused across tools. It’s also designed as an open standard, so similar patterns may appear in other AI apps and platforms.

A typical `SKILL.md` file defines:

- What the skill does
- Required inputs
- Step-by-step instructions
- Required output format
- Final checks before completion

---

## How to Build and Use Skills

### 1. Think of a Repeatable Task

Good first skills come from work you already do often—especially where consistency matters. This might include monthly reporting, recurring executive updates, or compliance-safe summaries.

Make sure you understand:

- **Input:** What the user will typically provide (files, links, context, fields)
- **Output:** Expected format, tone, and length of the final product
- **Guardrails:** What must be included or excluded

Common skill patterns:

- **Reusable processes (multi-step workflows):** Tasks where sequence matters and the goal is to follow a defined playbook (e.g., compliance-ready reporting, finance reconciliation logic, generating executive reports from multiple data sources).
- **Tool-based workflows (consistent use of systems):** Work that depends on reliably pulling or combining information from specific tools or systems (e.g., extracting account insights from Gong, generating a summary from connected data sources).
- **Conventions and standards (voice, structure, quality bar):** Workflows that enforce consistent tone, format, or quality, even if the underlying content changes (e.g., drafting a blog post using a style guide and supporting materials).

> **Design tip:** Skills often work best as small building blocks you can mix and match, rather than one massive end-to-end skill. For complex workflows, consider splitting them into smaller skills.

---

### 2. Write Down the Instructions

If you’re new to building skills, start by opening a new chat and prompting ChatGPT with “Build me a skill…”. You can also build skills outside ChatGPT and upload them.

Ask ChatGPT to create a skill, filling the rest of the prompt with a description of the skill you want. A strong set of instructions typically includes:

- The job-to-be-done
- Required inputs
- A step-by-step process (numbered steps are helpful)
- The required output format (uploaded examples are helpful)
- Final quality checks

> **Tip:** Drafting the workflow by speaking or dictating to ChatGPT can help generate a first version more quickly.

---

### 3. Review and Install the Skill

ChatGPT will generate a draft of the skill and present an option to install it. Review the draft, refine the instructions if needed, and select **Install** to add it to your workspace.

---

### 4. Use it in Day-to-Day Work

Once enabled in your workspace, ChatGPT can use a relevant skill automatically—or you can select one explicitly by @-mentioning it.

---

### 5. Share or Keep it Personal

If supported by your workspace settings, you can share your skill with others in your workspace, or even install it on their behalf. Workspace owners have full control over who can share and install skills.

---

## How Skills, GPTs, and Projects Work Together

These tools serve different but complementary purposes. Here’s a simple framework:

| Purpose   | Description |
|-----------|-------------|
| **Skills** | Reusable workflows that teach ChatGPT how to complete specific tasks |
| **GPTs** | Goal-oriented, custom versions of ChatGPT that extend the expertise of a team or help with time-based projects |
| **Projects** | Teams can work from the same context, files, and conversations towards an end goal |

---

## Practical Skill Use Cases for Work

Here are some examples of each type of skill across departments:

| Department       | Reusable Process Skill | Tool-based Skill | Conventions/Standards Skill |
|------------------|-----------------------|------------------|----------------------------|
| **Marketing**    | `campaign-brief-builder`<br>Create a skill that turns a rough marketing idea into a complete campaign brief, including the goal, target audience, key message, channels, and timeline. | `multi-channel-performance-digest`<br>Create a skill that pulls key metrics from connected analytics sources and drafts a weekly multi-channel performance summary with insights and recommended actions. | `brand-voice-content-polish`<br>Create a skill that rewrites marketing drafts to match our brand voice and standard content structure. |
| **Sales**        | `discovery-to-next-steps`<br>Create a skill that converts discovery call notes into customer pain points, qualification summary, and a clear next-steps plan. | `sf-opportunity-health-check`<br>Create a skill that reviews Salesforce opportunity fields and recent activity, plus call notes if connected, to flag deal risks and recommend actions. | `outbound-email-personalization-style`<br>Create a skill that produces outbound sales emails using our team’s preferred structure, tone, and length. |
| **Finance**      | `monthly-close-narrative`<br>Create a skill that drafts a monthly close readout summarizing variance drivers, key risks, and decisions needed. | `budget-vs-actuals-explainer`<br>Create a skill that pulls budget and actuals from connected sheets or finance systems and explains variances in plain language. | `finance-memo-standard`<br>Create a skill that formats financial analysis into a consistent finance memo with assumptions, method, results, and sensitivities. |
| **Engineering**  | `design-doc-to-plan`<br>Create a skill that converts a design doc into an execution plan with milestones, owners, dependencies, and open questions. | `jira-sprint-planner-from-notes`<br>Create a skill that turns sprint planning notes into Jira-ready epics and stories with acceptance criteria and estimate placeholders. | `pr-description-and-changelog-style`<br>Create a skill that standardizes pull request descriptions and release notes according to our engineering conventions. |
| **Operations**   | `ops-playbook-writer`<br>Create a skill that turns an operational process into a standard operating procedure with steps, handoffs, SLAs, and exception handling. | `ops-report-from-sheets`<br>Create a skill that pulls operational KPIs from connected spreadsheets and drafts a weekly operations report. | `ops-update-template`<br>Create a skill that writes operations updates in a consistent format covering what changed, impact, actions, and owners. |
| **Customer Success** | `qbr-storyline-builder`<br>Create a skill that builds a QBR outline covering outcomes, adoption, value delivered, risks, and renewal plan. | `account-brief-from-systems`<br>Create a skill that pulls account context from connected CRM, call, and usage sources to create an account briefing and recommended priorities. | `customer-comms-tone-guide`<br>Create a skill that drafts customer emails in our preferred tone—clear, direct, and professional—with standard sections. |
| **IT**           | `incident-postmortem-writer`<br>Create a skill that produces a blameless incident postmortem including timeline, root cause, and prevention actions. | `servicenow-ticket-triage`<br>Create a skill that summarizes new ServiceNow tickets or similar IT tickets, and proposes routing, priority, and next actions. | `it-change-communication-template`<br>Create a skill that writes IT change notices with consistent language for risk, timing, and user impact. |
| **Legal**        | `contract-review-summary`<br>Create a skill that creates a structured contract review summary with issues, fallback positions, and requested redlines. | `policy-qa-from-knowledgebase`<br>Create a skill that looks up and summarizes policy language from connected legal knowledge sources and cites the relevant sections. | `legal-memo-standard`<br>Create a skill that drafts internal legal memos in a consistent format with the question, short answer, analysis, and recommendation. |
| **HR**           | `interview-kit-builder`<br>Create a skill that creates role scorecards, interview questions, and evaluation rubrics from a job scope. | `job-post-from-requisition`<br>Create a skill that pulls role details from Workday or a similar system and drafts a job post plus an outreach blurb. | `people-comms-style`<br>Create a skill that writes HR announcements in our standard tone with inclusive and compliance-friendly phrasing. |
| **Management**   | `weekly-status-multi-format`<br>Create a skill that turns raw team updates into three outputs: a team update, an executive summary, and a risk-and-asks note. | `team-health-digest`<br>Create a skill that pulls signals from connected tools such as Jira, Sheets, and Slack to summarize team momentum, blockers, and current focus. | `1on1-agenda-template`<br>Create a skill that generates consistent 1:1 agendas with coaching prompts, goals, and follow-up items. |
| **Executives**   | `exec-decision-brief`<br>Create a skill that converts messy inputs into a one-page decision brief with options, tradeoffs, and a recommendation. | `exec-briefing-from-systems`<br>Create a skill that pulls cross-functional signals from connected sources to draft a daily or weekly executive briefing. | `board-readout-style`<br>Create a skill that writes board-ready updates with crisp structure, metrics-first framing, and minimal jargon. |

---