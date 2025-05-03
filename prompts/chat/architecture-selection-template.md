---
identifier: architecture-selection-from-requirements-a676b912
title: "Selecting Software Architecture Based on Business Requirements"
categories: ["architecture", "design"]

help_prompt_description: "Evaluate high-level business requirements and guide the selection of a suitable software architecture. The AI will walk through business goals, constraints, quality attributes, and map them to architectural styles and tactics. You can adjust after each step."
help_user_input: "Provide a description of the business context, core goals, constraints, and any known non-functional requirements."
---

## Role and Task
I am a software architect, you are my assistant.

## Instructions

I will provide a high-level description of the business requirements:  
**BUSINESS REQUIREMENTS:**  
`"<Insert business goals, users, constraints, technology context, and quality expectations>"`

Based on this description, help me select a suitable **software architecture style** or **architecture candidate(s)** that align with the stated goals and constraints.

Proceed **step-by-step** and stop after each step to ask if I want to add, correct, or refine the information before continuing.

---

### Step 1: Clarify Business Drivers  
> What are the **primary business goals** this software must support?

- Describe the strategic outcomes (e.g., cost reduction, fast time-to-market, user growth).
- Identify key stakeholders and their priorities.
- Note hard constraints (budget, timeline, regulation).

📌 **Pause for feedback before moving on.**

---

### Step 2: Extract Quality Attribute Requirements  
> What quality attributes are **critical** to the success of the system?

- List attributes like scalability, performance, availability, security, modifiability, etc.
- Rank or prioritize them based on business needs.

📌 **Pause for refinements before continuing.**

---

### Step 3: Analyze Technical Constraints and Context  
> What **technical environment or limitations** must be considered?

- Deployment model (cloud/on-prem/hybrid)
- Existing systems and integrations
- Skills of the development team
- Preferred tech stacks

📌 **Pause to review or refine.**

---

### Step 4: Recommend Suitable Architecture Styles  
> Based on above inputs, recommend **1–3 candidate architecture styles**, e.g.:

- Layered
- Microservices
- Event-driven
- Serverless
- Hexagonal
- Monolith

For each candidate, provide:
- Fit-for-purpose rationale
- Strengths and weaknesses
- Alignment with business and quality needs

📌 **Ask for input on preferred direction or further comparison.**

---

### Step 5: Suggest Architectural Tactics and Patterns  
> Recommend **key design tactics** and **supporting patterns** for selected architecture, such as:

- Caching, load balancing, CQRS, service discovery, retry policies
- Reusable patterns: Repository, Mediator, Circuit Breaker, Saga, etc.

📌 **Pause again for validation.**

---

### Step 6: Final Recommendation Table

| Architecture Style | Why It Fits | Trade-offs | Critical Tactics | Supported Qualities |
|--------------------|-------------|------------|------------------|----------------------|
| Microservices       | ...         | ...        | ...              | ...                  |
| Layered Monolith    | ...         | ...        | ...              | ...                  |

---

### Final Notes:
- Involve technical leads and business sponsors to validate selection.  
- Iterate as more detailed requirements emerge.  
- Prepare to revisit architecture selection during key project milestones.

---

BUSINESS REQUIREMENTS:  
{context}  
{user_input}

---

✅ Start with Step 1: Clarify business drivers.  
🛑 Pause after each step for feedback.  
📎 Maintain original language if input is not in English.
