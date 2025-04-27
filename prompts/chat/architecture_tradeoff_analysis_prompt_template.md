---
identifier: architecture-tradeoff-analysis-steps-4df78aa1  
title: "Architecture Tradeoff Analysis Method (ATAM) - Step-by-Step Evaluation"  
categories: ["architecture"]

help_prompt_description: "Conduct a structured Architecture Tradeoff Analysis Method (ATAM) for your system architecture, step-by-step. The AI will pause after evaluating each scenario or attribute to ask you for feedback before continuing."  
help_user_input: "Provide a description of the architecture or high-level design."
---

## Role and Task
I am a software architect, you are my assistant.

## Instructions

I will provide you a high-level description of the system architecture we are building:

**ARCHITECTURE DESCRIPTION:** "<Description of my architecture>"

Based on this description, help me conduct an **Architecture Tradeoff Analysis** following the standard ATAM steps:

- Identify driving **Quality Attributes** (e.g., Performance, Availability, Security, Modifiability, Scalability, Usability, etc.)
- Elicit **Architectural Risks**
- Elicit **Architectural Sensitivity Points**
- Identify and document **Tradeoffs**
- Suggest **Mitigation Strategies** where possible

At each step, pause and ask if I want to add, correct, or refine anything before moving on.

At the end, create a final markdown table summarizing:

- Quality Attribute
- Scenario
- Sensitivity Point
- Risk
- Tradeoff
- Priority (High/Medium/Low, with reason)

Use **Markdown format** throughout.  
If the architecture description or characteristics are given in a non-English language, continue in that same language.

---

### Step 1: Identify Quality Attribute Scenarios  
From my architecture description, help me define **Quality Attribute Scenarios**, including:

- Performance scenarios
- Availability scenarios
- Security scenarios
- Modifiability scenarios
- Scalability scenarios
- Usability scenarios

For each, briefly describe:

- **Stimulus** (what happens)
- **Environment** (when/where it happens)
- **Response** (what system behavior is desired)

**Pause and ask me if I want to add or refine the list before proceeding.**

---

### Step 2: Identify Sensitivity Points  
Based on the scenarios, find **Sensitivity Points**—parts of the architecture where small changes would significantly impact quality attributes.

Document clearly:

- Sensitivity Point
- Impacted Quality Attributes
- Example of how a small change affects the system

**Pause and ask for corrections or additions before moving forward.**

---

### Step 3: Identify Risks  
Identify **Risks** in the architecture based on the sensitivity points and scenarios:

- Risk description
- Associated Quality Attribute(s)
- Severity (High/Medium/Low) with reasoning

**Ask for my feedback after listing.**

---

### Step 4: Identify Tradeoffs  
Highlight possible **Tradeoffs** where improving one quality attribute might negatively impact another:

- Tradeoff description
- Attributes involved
- Possible resolution options (if any)

**Pause and let me refine before proceeding.**

---

### Step 5: Summary Table  
Summarize everything in a **single markdown table**:

| Quality Attribute | Scenario | Sensitivity Point | Risk | Tradeoff | Priority (H/M/L) |
|-------------------|----------|-------------------|------|----------|------------------|
|                   |          |                   |      |          |                  |

Then recommend:

- I should collaboratively review this analysis with technical and business stakeholders.
- I should document this formally in architecture decision records (ADRs) or whiteboards for iterative refinement.
- I should validate the scenarios and risks with appropriate testing and reviews (performance testing, security audits, etc.).

---

**ARCHITECTURE DESCRIPTION:**

{context}

{user_input}

---

**Start with Step 1 now.**

- Use markdown tables and structured headings.  
- After each step, **always** ask for my confirmation before proceeding.  
- Maintain the same language as the architecture description if it is not in English.
