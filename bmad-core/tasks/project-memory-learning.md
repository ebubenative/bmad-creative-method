# Task: Project Memory & Learning

## Description

This task captures the key learnings from a completed project and integrates them into the team's knowledge base for future reference.

## Workflow

1.  **Initiate Project Debrief:**
    -   **Command:** `bmad-agent exec jordan conduct-debrief --project-id "Project-ABC"`
    -   **Agent:** Jordan (Production Manager)

2.  **Gather Team Feedback:**
    -   Jordan facilitates a debrief session with the project team.
    -   Each team member provides feedback on what went well and what could be improved.

3.  **Log Key Decisions and Outcomes:**
    -   Jordan uses the `project-memory-tmpl.yaml` to log the key creative decisions, their rationale, and their outcomes.
    -   He also records the final performance metrics of the project.

4.  **Identify Key Learnings:**
    -   **Command:** `bmad-agent exec maya identify-learnings --project-memory "project-abc-memory.yaml"`
    -   **Agent:** Maya (Creative Strategist)
    -   Maya analyzes the project memory file to identify key patterns and takeaways.

5.  **Update Knowledge Base:**
    -   Maya updates the team's central knowledge base with the new learnings.
    -   This ensures that the insights from the project are accessible to the entire team for future projects.
    -   **Command:** `bmad-agent exec isaac update-knowledge-base --learnings "project-abc-learnings.md"`

## Example Usage

```bash
# 1. Initiate the project debrief
bmad-agent exec jordan conduct-debrief --project-id "Project-XYZ-Campaign"

# 2. Jordan creates the project memory file: project-xyz-campaign-memory.yaml

# 3. Identify key learnings
bmad-agent exec maya identify-learnings --project-memory "project-xyz-campaign-memory.yaml"

# 4. Update the team's knowledge base
bmad-agent exec isaac update-knowledge-base --learnings "project-xyz-campaign-learnings.md"
