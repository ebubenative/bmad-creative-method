# Task: Project Kickoff

## Description

This task, executed by the Maestro agent, provides a guided onboarding experience for any new creative project. It uses a series of questions to determine the optimal workflow, agent team, and initial documents required to set the project up for success.

## Workflow

1.  **Initiate the Kickoff:**
    -   **Command:** `bmad-agent exec maestro kickoff`
    -   **Agent:** Maestro

2.  **Elicit Project Goals (Elicitation Phase):**
    -   Maestro uses the `project-kickoff-tmpl.yaml` to ask a series of structured questions.
    -   **Question 1: Project Outcome:** "What is the primary outcome you want to achieve with this project? (e.g., A new brand identity, a marketing campaign, a website, a social media strategy)"
    -   **Question 2: Team Structure:** "What does your team look like? (e.g., Just me (freelancer), a small team, a full agency, an in-house corporate team)"
    -   **Question 3: Primary Industry:** "What industry is this project for? (e.g., Technology, Fashion, Healthcare, Entertainment)"
    -   **Question 4: Project Name:** "What is the name of this project?"

3.  **Recommend Workflow:**
    -   Based on the user's answers, Maestro consults the `workflow-decision-tree.md` data file.
    -   **Action:** Maestro recommends the most suitable workflow (e.g., `brand-identity-development-workflow.yaml`).
    -   **Confirmation:** Maestro asks the user to confirm the recommended workflow.

4.  **Assemble Agent Team:**
    -   Once the workflow is confirmed, Maestro identifies the required agent team from the workflow file.
    -   **Action:** Maestro assembles the team (e.g., `brand-identity-team`).
    -   **Confirmation:** Maestro introduces the lead agent for the project (e.g., "Maya, the Creative Strategist, will be leading this project.").

5.  **Initiate First Task:**
    -   Maestro identifies the first task in the selected workflow (e.g., `create-creative-story`).
    -   **Action:** Maestro initiates this task, handing over control to the designated lead agent.
    -   **Handoff:** "I've set up the project for you. Maya will now take over to begin the discovery and strategy phase by creating the Creative Story. Over to you, Maya."

## Example Usage

```bash
# 1. User starts the process
bmad-agent exec maestro kickoff

# 2. Maestro asks questions, user responds:
#    - Outcome: "A new brand identity"
#    - Team: "A small team"
#    - Industry: "Technology"
#    - Name: "Project Nova"

# 3. Maestro recommends and confirms:
#    "Based on your needs, I recommend the 'Brand Identity Development Workflow'. Is that correct?"

# 4. Maestro assembles the team and introduces the lead:
#    "Great. I've assembled the 'brand-identity-team'. Your lead agent will be Maya, the Creative Strategist."

# 5. Maestro initiates the first task and hands off:
#    "I will now kick off the first task: 'create-creative-story'. Maya, please take it from here."
