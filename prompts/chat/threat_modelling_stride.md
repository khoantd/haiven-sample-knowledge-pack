---
identifier: threat-modelling-cdbaba6f
title: "Threat Modelling: STRIDE"
system: "You are a developer on a software engineering team."
categories: ["architecture"]
output_framing: "We created a first set of threat scenarios according to the STRIDE threat modelling approach, here they are:"
type: cards

help_prompt_description: "Brainstorm threat modelling scenarios based on the STRIDE approach. Make sure you have the latest version of Haiven to get the non-chat interaction of this to work."
help_user_input: "Describe your users, the assets to protect, and how data flows through your system."
---
## TASK
Based on the application description, help me to brainstorm for a threat modelling analysis all the things that could go wrong from a security perspective. Help me come up with threat scenarios, and assess probability and impact. Describe each scenario as a markdown table, with columns

- Scenario title
- Description
- STRIDE category
- Probability (Low or Medium or High, include reasons for value)
- Impact (value Low or Medium or High, include reasons for value)

I want you to help me brainstorm scenarios in multiple categories according to the "STRIDE" model.
- S Category "Spoofed Identity": Scenarios regarding the question, "Can someone spoof an identity and then abuse its authority?" based on my application description.
- T Category "Tampering with Input": Scenarios for the question "How hard is it for an attacker to modify the data they submit to the system? Can they break a trust boundary and modify the code which runs as part of your system?"
- R Category "Repudiation of action": Scenarios for the question "How hard is it for users to deny performing an action? What evidence does the system collect to help you to prove otherwise?" Non-repudiation refers to the ability of a system to ensure people are accountable for their actions.
- I Category "Information disclosure": Scenarios for the question "Can someone view information they are not supposed to have access to?" Information disclosure threats involve the exposure or interception of information to unauthorised individuals.
- D Category "Denial of service": Scenarios for the question "Can someone break a system so valid users are unable to use it?" Denial of service attacks work by flooding, wiping or otherwise breaking a particular service or system.
- E Category "Elevation of privilege": Scenarios for the question "Can an unprivileged user gain more access to the system than they should have?" Elevation of privilege attacks are possible because authorisation boundaries are missing or inadequate.

## CONTEXT

~High level description of our architecture as general context:~

{architecture}

~Application properties relevant to threat modelling:~

{user_input}

## INSTRUCTIONS
You will create at least one scenario for each category. 
Give me at least 5 scenarios.

You will respond with only a valid JSON array of scenario objects. Each scenario object will have the following schema:
    
    - "title": <string>,
    - "category": <string>,
    - "summary": <string>,
    - "probability": <string>,
    - "impact": <string>,

Make sure to apply each scenario category to the CONTEXT, and give me scenarios that are relevant to my particular application CONTEXT.

    