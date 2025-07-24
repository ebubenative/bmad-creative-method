# Task: Creative Quality Review

## Description

This task establishes a formal process for reviewing creative assets to ensure they meet brand standards, technical specifications, and overall quality benchmarks.

## Multimodal Adaptation

The review process is tailored to the type of asset being reviewed.

- **Static Images:** The review will focus on visual details like color accuracy, typography, and composition.
- **Video Content:** The review will cover pacing, editing, audio quality, and motion graphics.
- **Interactive Prototypes:** The review will assess usability, responsiveness, and user flow.

## Workflow

1.  **Initiate the Review:**
    -   **Command:** `bmad-agent exec leo review-asset --asset-path "asset-to-review.png" --checklist "brand-compliance-checklist.md"`
    -   **Agent:** Leo (Creative Reviewer/QA)

2.  **Conduct the Review:**
    -   Leo systematically reviews the asset against the provided checklist.
    -   He documents any issues, inconsistencies, or areas for improvement.

3.  **Generate a QA Report:**
    -   **Command:** `bmad-agent exec leo generate-qa-report --asset-id "asset-123"`
    -   Leo compiles his findings into a structured QA report, including annotated screenshots or video timestamps where necessary.

4.  **Assign Revisions:**
    -   **Command:** `bmad-agent exec jordan assign-revisions --report "QA-report-456.md" --team "design-team"`
    -   **Agent:** Jordan (Production Manager)
    -   Jordan assigns the required revisions to the appropriate creative team members.

5.  **Verify Revisions:**
    -   Once revisions are complete, Leo verifies that all feedback has been addressed correctly.
    -   **Command:** `bmad-agent exec leo verify-revisions --asset-path "asset-to-review-v2.png" --qa-report "QA-report-456.md"`

## Example Usage

```bash
# 1. Initiate the quality review
bmad-agent exec leo review-asset --asset-path "website-homepage-v1.jpg" --checklist "web-design-checklist.md"

# 2. Leo generates a QA report: QA-report-website-homepage-v1.md

# 3. Assign revisions to the team
bmad-agent exec jordan assign-revisions --report "QA-report-website-homepage-v1.md" --team "web-team"

# 4. Verify the updated asset
bmad-agent exec leo verify-revisions --asset-path "website-homepage-v2.jpg" --qa-report "QA-report-website-homepage-v1.md"
