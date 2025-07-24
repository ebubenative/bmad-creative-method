# Task: Mood Board Creation

## Description

This task guides the creation of a mood board to visually explore the look and feel of a creative project. It leverages the `mood-board-tmpl.yaml` to structure the output.

## Multimodal Adaptation

This task is inherently multimodal, focusing on the collection and curation of visual assets. The process adapts based on the nature of the project and the available inputs.

- **If the input is a detailed creative brief:** The task will focus on finding visuals that align with the described aesthetic and strategic goals.
- **If the input is a set of keywords:** The task will involve a broader exploration of visual themes related to those keywords.
- **If the input includes existing brand assets:** The task will incorporate those assets and find complementary visuals.

## Workflow

1.  **Initiate the Task:**
    -   **Command:** `bmad-agent exec isaac gather-inspiration --topic "Project-XYZ-Mood-Board"`
    -   **Agent:** Isaac (Creative Researcher)

2.  **Populate the Mood Board Template:**
    -   Isaac uses the `mood-board-tmpl.yaml` to structure the collected assets.
    -   He populates the `Key Images`, `Color Palette`, `Typography Samples`, and `Texture & Pattern` fields.
    -   He also adds `Descriptive Words` to capture the intended mood.

3.  **Review and Refine:**
    -   **Command:** `bmad-agent exec adrian review-mood-board --file "Project-XYZ-Mood-Board.yaml"`
    -   **Agent:** Adrian (Creative Director)
    -   Adrian reviews the mood board and provides feedback for refinement.

4.  **Finalize the Mood Board:**
    -   Isaac incorporates Adrian's feedback and finalizes the mood board.
    -   The final mood board is saved and linked to the project.

## Example Usage

```bash
# 1. Initiate mood board creation
bmad-agent exec isaac gather-inspiration --topic "New-Mobile-App-Launch"

# 2. Isaac creates the mood board file: New-Mobile-App-Launch-Mood-Board.yaml

# 3. Review the mood board
bmad-agent exec adrian review-mood-board --file "New-Mobile-App-Launch-Mood-Board.yaml"
