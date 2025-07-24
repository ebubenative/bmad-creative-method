# Workflow Decision Tree

This document provides a simple decision-making framework for the Maestro agent to recommend the appropriate workflow based on user inputs.

## Logic

The logic is a series of `if-then` conditions. The Maestro agent will parse this file to find the best match.

---

### **Brand & Identity**

-   **IF** `outcome` contains "brand identity" OR "rebrand" OR "logo"
-   **THEN** recommend `brand-identity-development-workflow.yaml`

---

### **Marketing & Campaigns**

-   **IF** `outcome` contains "campaign" OR "advertisement" OR "commercial"
-   **THEN** recommend `campaign-creation-workflow.yaml`

-   **IF** `outcome` contains "commercial" AND ("video" OR "film")
-   **THEN** recommend `commercial-production-workflow.yaml`

---

### **Digital Products**

-   **IF** `outcome` contains "website" OR "web app" OR "mobile app" OR "digital product"
-   **THEN** recommend `digital-product-design-workflow.yaml`

---

### **Content & Social Media**

-   **IF** `outcome` contains "social media" OR "content creator" OR "influencer"
-   **THEN** recommend `content-creator-workflow.yaml`

---

### **Solo & Small Teams**

-   **IF** `team_structure` is "Just me" OR "freelancer"
-   **THEN** recommend `solo-creative-workflow.yaml` (unless a more specific outcome is chosen)

---

### **Studio & Agency**

-   **IF** `team_structure` is "small team" OR "full agency" OR "in-house"
-   **THEN** recommend `studio-collaborative-workflow.yaml` (as a general purpose option if no specific outcome is chosen)

---

## Fallback

-   **IF** no specific match is found
-   **THEN** recommend `studio-collaborative-workflow.yaml` as the default comprehensive option and ask the user for clarification.
