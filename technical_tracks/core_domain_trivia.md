# 🔍 FeBe Technical Track: Core Domain Trivia & Code Review Collaboration

**Best Suited For:** Mid-Level / Core Engineers
**Target Evaluation:** Code comprehension, architectural empathy, debugging instincts, and peer-to-peer technical collaboration.

---

## 🚫 The Anti-Patterns to be aware of
* **No Syntax Traps:** Do not quiz candidates on obscure language trivia or esoteric framework features that can be looked up in two seconds on MDN or StackOverflow.
* **No Defensive Gatekeeping:** If a candidate suggests a valid refactoring pattern that differs from how your team currently writes code, do not penalize them. Grade on their justification, not their compliance with your personal aesthetic preference.
* **No Linear Script Reading:** Do not let the round devolve into the candidate quietly reading code line-by-line. It must be an active, collaborative discussion.

---

## 🛠️ The FeBe Alternative: The "Real-World PR Review"

Instead of forcing a candidate to write a script from scratch while an interviewer watches them type, provide the candidate with a realistic, pre-written Pull Request (PR) containing roughly 50 to 150 lines of code. 

This PR should intentionally mirror your company's actual technical ecosystem and contain a mix of logical bugs, structural anti-patterns, and architectural flaws.

### Pre-Interview Disclosure Example:
As recommended by the "No Hidden Traps" principle, the interviewer must specify the runtime paradigms to be evaluated at least 5 business days in advance:
> *"We will be reviewing a legacy Pull Request with a heavy focus on debugging async/await concurrency and handling race conditions."*

### The Interview Structure (60 Minutes)
1. **The Briefing (10 Mins):** Provide a brief overview of the feature's business goal (e.g., *"This PR implements a new background worker to sync customer billing statuses with our payment processor"*). Give the candidate access to the code.
2. **The Collaborative Review (35 Mins):** The candidate walks through the code out loud, pointing out issues, explaining *why* they are problematic, and discussing how to fix them. 
3. **The Embedded Behavioral Pivot (15 Mins):** The interviewer pushes back on a finding or introduces a changing requirement to test real-world collaboration and pragmatism.

---

## 💡 Engineering Disclosures (What to Bake into the Code)
To extract a high-fidelity execution signal, the sample code should contain specific structural issues across three tiers:
* **Tier 1: High-Impact Execution Flaws:** An obvious race condition, an N+1 database query, a missing error boundary around an external API call, or unhandled asynchronous rejections.
* **Tier 2: Code Maintainability Issues:** Tight coupling, poorly named abstractions, hardcoded environmental configurations, or a total lack of test coverage for a critical edge case.
* **Tier 3: The Embedded Behavioral Signal:** Include a section of code that is technically functional but highly over-engineered (e.g., an unnecessary abstraction layer or a premature optimization). Observe if the candidate pragmatically recommends simplifying it for the sake of delivery speed.

---

## 📊 Objective Code Review Rubric (Pass / Fail Metrics)

Evaluation must be grounded strictly in engineering execution, diagnostic clarity, and healthy communication.

| Evaluation Pillar | Green Flags (Pass) | Red Flags (Fail) |
| :--- | :--- | :--- |
| **Diagnostic Accuracy** | Successfully identifies critical performance bottlenecks (e.g., the N+1 query) or system vulnerabilities (e.g., unhandled API crashes) and accurately explains the operational consequences. | Misses foundational execution flaws entirely, focusing exclusively on trivial cosmetic details like spacing, comment styles, or minor syntax choices. |
| **Architectural Empathy & Clarity** | Explains *why* a structural change is needed by framing it around long-term maintenance, readability, and team velocity. Offers concrete, actionable alternatives. | Dictates corrections dogmatically without explaining the reasoning, uses condescending language, or struggles to articulate how code modifications impact the broader system. |
| **Collaborative Receptivity** | Engages in a healthy, constructive dialogue when the interviewer introduces alternative viewpoints or constraints; treats the session as a peer alignment meeting. | Becomes visibly defensive or unyielding when code choices are challenged, or demonstrates an inability to compromise on "perfect code" when a business constraint is introduced. |

**Final Calculation:** To advance, the candidate must achieve a "Green Flag" across all three pillars.
