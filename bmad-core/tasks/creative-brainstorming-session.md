# Task: Creative Brainstorming Session

## Description

This task facilitates a structured brainstorming session to generate creative ideas for a project. It can be run with a solo agent or a team of agents.

## Multimodal Adaptation

This task can be adapted to different brainstorming techniques and inputs.

- **Text-Based Brainstorming:** Agents can generate ideas in a shared document.
- **Visual Brainstorming:** Agents can contribute to a shared digital whiteboard with images, sketches, and notes.
- **Hybrid Brainstorming:** The session can combine both text and visual elements.

## Workflow

1.  **Initiate the Session:**
    -   **Command:** `bmad-agent exec maya facilitate-brainstorming --topic "Campaign-Slogan-Ideas"`
    -   **Agent:** Maya (Creative Strategist)

2.  **Set the Stage:**
    -   Maya provides the team with the creative brief and any relevant research.
    -   She outlines the brainstorming technique to be used (e.g., round-robin, mind mapping).

3.  **Generate Ideas:**
    -   The participating agents generate and share their ideas.
    -   **Example Agents:**
        -   Alex (Copywriter) generates slogan ideas.
        -   Gabriel (Graphic Designer) sketches visual concepts.
        -   Adrian (Creative Director) provides high-level creative direction.

4.  **Review and Cluster Ideas:**
    -   Maya reviews all generated ideas and clusters them into themes.
    -   The team discusses the clustered ideas and identifies the most promising concepts.

5.  **Synthesize and Document:**
    -   Maya synthesizes the session's output into a summary document.
    -   The document includes the top ideas, key discussion points, and next steps.

## Example Usage

```bash
# 1. Initiate the brainstorming session
bmad-agent exec maya facilitate-brainstorming --topic "New-Product-Launch-Campaign" --team "campaign-development-team"

# 2. The team collaborates to generate ideas.

# 3. Maya creates a summary document: New-Product-Launch-Campaign-Brainstorm-Summary.md
