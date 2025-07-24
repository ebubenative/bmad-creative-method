# Task: Client Feedback Integration

## Description

This task outlines the process for receiving, interpreting, and integrating client feedback into a creative project.

## Multimodal Adaptation

The task adapts to the format of the client feedback.

- **Written Feedback:** The task will parse emails or documents for actionable comments.
- **Verbal Feedback:** The task will use speech-to-text to transcribe and summarize feedback from calls or meetings.
- **Visual Feedback:** The task will involve annotating images or video with the client's comments.

## Workflow

1.  **Receive Feedback:**
    -   **Command:** `bmad-agent exec chloe receive-feedback --source-type "email" --file "client-feedback.eml"`
    -   **Agent:** Chloe (Client Liaison)

2.  **Process and Interpret Feedback:**
    -   Chloe processes the feedback, clarifying any ambiguous points with the client if necessary.
    -   She translates the client's feedback into a clear, actionable list of revisions.

3.  **Create a Revision Plan:**
    -   **Command:** `bmad-agent exec jordan create-revision-plan --feedback-summary "revision-list.md"`
    -   **Agent:** Jordan (Production Manager)
    -   Jordan creates a plan for implementing the revisions, assigning tasks to the appropriate team members.

4.  **Execute Revisions:**
    -   The creative team executes the revisions based on the plan.

5.  **Present Revised Creative:**
    -   **Command:** `bmad-agent exec chloe present-creative --project-id "Project-ABC" --version "v3"`
    -   Chloe presents the revised creative work to the client for final approval.

## Example Usage

```bash
# 1. Receive client feedback
bmad-agent exec chloe receive-feedback --source-type "video" --file "client-feedback-call.mp4"

# 2. Chloe processes the feedback and creates a summary: revision-summary.md

# 3. Create a revision plan
bmad-agent exec jordan create-revision-plan --feedback-summary "revision-summary.md"

# 4. The team executes the revisions.

# 5. Present the revised work
bmad-agent exec chloe present-creative --project-id "Project-ABC" --version "v3"
