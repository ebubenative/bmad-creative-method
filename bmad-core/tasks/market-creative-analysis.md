# Task: Market Creative Analysis

## Description

This task analyzes the creative output of competitors and the broader market to identify trends, opportunities, and best practices.

## Multimodal Adaptation

This task adapts to the type of creative being analyzed.

- **Website Analysis:** The task will involve scraping and analyzing the design, UX, and copy of competitor websites.
- **Social Media Analysis:** The task will focus on the visual and messaging strategies of competitors on social media platforms.
- **Campaign Analysis:** The task will deconstruct the creative elements of major campaigns in the market.

## Workflow

1.  **Initiate the Analysis:**
    -   **Command:** `bmad-agent exec isaac conduct-trend-analysis --industry "your-industry" --domain "your-domain"`
    -   **Agent:** Isaac (Creative Researcher)

2.  **Gather Data:**
    -   Isaac gathers a wide range of creative examples from competitors and the market.
    -   This can include website screenshots, social media posts, ad campaigns, and more.

3.  **Analyze and Synthesize:**
    -   Isaac analyzes the collected data, looking for patterns in visual style, messaging, and strategy.
    -   He synthesizes his findings into a market creative analysis report.

4.  **Present Findings:**
    -   **Command:** `bmad-agent exec maya present-findings --report "market-creative-analysis.md"`
    -   **Agent:** Maya (Creative Strategist)
    -   Maya presents the findings to the creative team, highlighting key insights and strategic recommendations.

## Example Usage

```bash
# 1. Initiate the analysis
bmad-agent exec isaac conduct-trend-analysis --industry "fast-food" --domain "social-media-campaigns"

# 2. Isaac creates the analysis report: fast-food-social-media-analysis.md

# 3. Present the findings
bmad-agent exec maya present-findings --report "fast-food-social-media-analysis.md"
