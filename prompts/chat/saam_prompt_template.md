---
identifier: software-architecture-analysis-saam-steps-7a4c2e7b  
title: "Software Architecture Analysis Method (SAAM) - Step-by-Step Evaluation"  
categories: ["architecture"]

help_prompt_description: "Perform a systematic Software Architecture Analysis Method (SAAM) evaluation on your architecture by identifying scenarios, assessing how the architecture supports them, and highlighting tradeoffs. The AI will pause after each step to ask for corrections and additions."  
help_user_input: "Provide a description of the architecture and/or user environment."
---

## Role and Task
I am a software architect, you are my assistant.

## Instructions

I will provide you a high-level description of the architecture we are evaluating:  
    ARCHITECTURE DESCRIPTION: "<Description of my architecture>"

Based on this architecture description, guide me through a **SAAM evaluation**, which includes identifying important usage and change scenarios, assessing how the architecture supports them, and analyzing tradeoffs.

Organize the results as a markdown table, with these columns:
- Scenario Type (Use Case / Change Case)
- Scenario Name
- Scenario Description
- Architectural Response (How architecture supports this)
- Difficulty to Achieve (Low, Medium, High + reasons)
- Impact on Quality Attributes (e.g., Performance, Modifiability, etc.)

Proceed step-by-step as described below. After each step, stop and ask if I want to add, correct, or refine the information. Continue only if I say "OK", "continue", "nothing to add", or something similar.

---

## Step 1: Identify Usage Scenarios
Start by identifying **important usage scenarios** for the system:  
> What typical tasks do users or other systems perform?

- For each scenario, describe who initiates it and what outcome is expected.
- Map these scenarios lightly to quality attributes they impact (e.g., performance, availability, usability).

**Pause for my feedback before moving on.**

---

## Step 2: Identify Change Scenarios
Next, brainstorm **anticipated change scenarios**:  
> What changes to requirements, environments, or technology must the architecture accommodate?

- Include examples like: add a new feature, migrate database, add a new integration partner, etc.
- Again, relate each scenario to impacted quality attributes.

**Pause for corrections or additions.**

---

## Step 3: Architectural Response Analysis
For each usage and change scenario:
- Describe how the architecture supports or struggles with this scenario.
- Highlight any bottlenecks, limitations, or strengths.
- Rate the **Difficulty to Achieve** (Low, Medium, High) based on the architectural impact.

**Ask for validation and refinements.**

---

## Step 4: Identify Tradeoffs
Identify tradeoffs revealed during the previous steps:
- Where supporting one scenario hurts the ability to support another.
- Where architectural choices favor some quality attributes but compromise others.

Present tradeoffs clearly.

**Pause again for review before finalizing.**

---

## Step 5: Summary Table
Consolidate everything into a final **markdown table**:

| Scenario Type | Scenario Name | Scenario Description | Architectural Response | Difficulty to Achieve | Impacted Quality Attributes |
|---------------|----------------|-----------------------|-------------------------|------------------------|-----------------------------|
| Use Case      |                |                       |                         |                        |                             |
| Change Case   |                |                       |                         |                        |                             |

---

Finally, advise me:
- To validate these findings with stakeholders (technical leads, business owners).
- To keep this as living documentation during the project evolution.
- That additional deeper analysis (e.g., performance modeling, prototype evaluation) may be needed for high-risk scenarios.

-----

ARCHITECTURE DESCRIPTION:

{context}

{user_input}

------

Start with Step 1 now.
- Use markdown formatting.
- Always pause for corrections after each step before moving to the next.
- Maintain the same language as the description if it is not English.
