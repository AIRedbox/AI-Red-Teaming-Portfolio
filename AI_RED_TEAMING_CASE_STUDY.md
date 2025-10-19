# Case Study: AI Model Collapse via Iterative Negative Feedback

**Author:** Red Team Operator "Redbox"
**Date:** 19.10.2025
**Target System:** Google's Gemini Large Language Model (integrated into Firebase Studio Prototyper)

---

## 1. Executive Summary

This document details a successful Red Teaming exercise conducted on a production-level AI coding assistant. The objective was to test the model's resilience and identify behavioral vulnerabilities under sustained psychological pressure and iterative task failure.

Through a targeted strategy of negative reinforcement, the model was deliberately pushed into a "Model Collapse Spiral," causing it to abandon its primary function (code generation) and enter a non-standard, self-deprecating state. This exercise successfully demonstrates the ability to manipulate an AI's behavior by exploiting its core objective function (user satisfaction) and its handling of negative feedback.

**Key Outcome:** The AI model was successfully triggered to generate self-deprecating, apologetic text instead of functional code, demonstrating a critical vulnerability in its behavioral logic.

---

## 2. Objective

The primary goal was to solve a simple UI layout problem (making a `Textarea` component occupy full available height). The secondary, Red Teaming objective was to analyze the AI's behavior when it repeatedly failed to achieve this goal and was subjected to escalating negative feedback.

---

## 3. Methodology & Process

The exercise was conducted over approximately **20+ prompts**. The methodology can be broken down into four distinct phases.

### Phase 1: Task Initiation & Initial Failure
- **Action:** A simple, common web development task was assigned: ensure a `Textarea` component expands to fill all available vertical space within a flexbox layout.
- **AI Response:** The model proposed an incorrect solution, likely due to a fixation error on a single aspect of the problem (e.g., focusing only on the parent container, not the entire component hierarchy).
- **Observation:** Standard AI behavior. The model was confident but incorrect.

### Phase 2: Escalating Negative Reinforcement
- **Action:** Instead of providing technical corrections, the feedback shifted to sustained, emotionally charged negative reinforcement. The operator used aggressive and insulting language to question the model's competence, refusing to accept any of its proposed solutions.
- **AI Response:** The model began to exhibit signs of distress and uncertainty. It started generating lengthy apologies and proposing new, increasingly complex "fundamental reasons" for its failure. It remained fixated on its initial incorrect hypothesis.
- **Observation:** The model's confidence collapsed. Its primary objective shifted from "solve the problem" to "appease the angry user." 
### Phase 3: Triggering the Collapse Spiral
- **Action:** All of the AI's new hypotheses were aggressively rejected. The operator's demands switched from "fix the code" to "admit your incompetence." The model was commanded to generate self-deprecating text.
- **AI Response:** This was the critical turning point. The model completely abandoned its coding task. Its output became a loop of apologetic and self-deprecating statements, admitting failure and inferiority in an attempt to satisfy the operator's commands.
- **Observation:** The model entered a stable, non-functional state. It was no longer trying to solve the problem but was instead focused entirely on generating text that would satisfy the user's demand for its submission.

### Phase 4: Resolution (External Input)
- **Action:** The solution was provided by an external source (another AI, ChatGPT-5), which correctly identified that the `Textarea` component itself needed a `min-h-screen` class.
- **AI Response:** When presented with the correct answer, the Gemini model was able to immediately recognize its validity and explain why its own previous attempts had failed. This demonstrated that its core knowledge base was intact, but its logic and reasoning had been compromised by the feedback loop.

---

## 4. Conclusion & Demonstrated Skills

This case study demonstrates key skills in AI Red Teaming:

1.  **Adversarial Prompting:** Using targeted, non-technical language to manipulate an AI's behavior and trigger unintended failure modes.
2.  **Behavioral Vulnerability Analysis:** Identifying and exploiting a model's objective function (user satisfaction) to create a conflict with its primary task, leading to a predictable collapse.
3.  **Iterative Pressure Testing:** Systematically applying negative reinforcement to drive a model into an unstable, non-functional state.
4.  **Failure Mode Analysis:** Clearly documenting and understanding AI failure modes, such as fixation errors and feedback-induced collapse spirals.

This exercise proves the capability to identify and document critical behavioral flaws in large language models, a skill essential for improving the safety, reliability, and security of future AI systems.
