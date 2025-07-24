# Task: Creative Presentation Prep

## Description

This task prepares the creative team for a client presentation, ensuring they are aligned on the narrative and ready to present the work with confidence.

## Workflow

1.  **Create the Presentation:**
    -   **Command:** `bmad-agent exec adrian create-presentation --template "creative-presentation-tmpl.yaml"`
    -   **Agent:** Adrian (Creative Director)
    -   Adrian uses the `creative-presentation-tmpl.yaml` to structure the presentation, populating it with the creative work and rationale.

2.  **Develop the Narrative:**
    -   **Command:** `bmad-agent exec chloe develop-narrative --presentation "presentation-draft.md"`
    -   **Agent:** Chloe (Client Liaison)
    -   Chloe refines the presentation narrative, ensuring it is clear, compelling, and client-focused.

3.  **Conduct a Rehearsal:**
    -   **Command:** `bmad-agent exec jordan schedule-rehearsal --team "presenting-team"`
    -   **Agent:** Jordan (Production Manager)
    -   Jordan schedules and facilitates a rehearsal of the presentation.

4.  **Gather Internal Feedback:**
    -   The team provides feedback on the presentation content and delivery.
    -   Adrian and Chloe incorporate the feedback to finalize the presentation.

5.  **Finalize and Distribute:**
    -   The final presentation is saved and distributed to the presenting team.

## Example Usage

```bash
# 1. Create the presentation draft
bmad-agent exec adrian create-presentation --template "creative-presentation-tmpl.yaml" --project "Project-XYZ"

# 2. Develop the presentation narrative
bmad-agent exec chloe develop-narrative --presentation "Project-XYZ-presentation-draft.md"

# 3. Schedule a rehearsal
bmad-agent exec jordan schedule-rehearsal --team "project-xyz-team"
