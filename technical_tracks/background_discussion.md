# 🗣️ FeBe Technical Track: Background Architecture Discussion

**Best Suited For:** Senior, Staff, and Principal Engineers
**Target Evaluation:** Real-world delivery retrospection, production empathy, operational maturity, and technical ownership.

---

## 🚫 The Anti-Patterns to be aware of
* **No Fictional Canvas Prompts:** This is *not* a system design round where the candidate draws an imaginary setup on a whiteboard. It is a strict historical analysis of real systems they have actually shipped to production.
* **No High-Level Hand-Waving:** If a candidate cannot drill down into the specific schema choices, background job configurations, or actual network bottlenecks of their own architecture, they did not lead the execution. 
* **No "Perfect Architecture" Posturing:** Do not reward candidates who try to pretend their past systems never broke. Reward the analytical honesty of engineers who openly discuss their production failures and what they learned from them.

---

## 🛠️ The FeBe Alternative: The Deconstructive Review

The entire round focuses on a significant architectural project the candidate listed on their resume or highlighted in their initial application. The interviewer's job is to act as an investigative engineering partner, digging past the high-level diagrams to discover how the system actually survived in production.

### Pre-Interview Disclosure Example:
As recommended by the "No Hidden Traps" principle, the interviewer must specify the operational domains to be discussed at least 5 business days in advance:
> *"For our background discussion, we will be diving deep into the [Candidate's Specific Project]. Please come prepared to walk us through how you handled database connection management, caching invalidation strategies, and third-party API partial failures under peak load."*

### The Interview Structure (60 Minutes)
1. **The System Genesis (15 Mins):** Map out the baseline architecture. What were the initial business requirements, what constraints did the team face, and what compromises were made to hit the shipping deadline?
2. **The Production Reality (25 Mins):** Drill into the technical bottlenecks. Once users hit the system at scale, where did the architecture fracture first? How did the engineering team diagnose, isolate, and systematically fix those issues?
3. **The Technical Debt Retro (20 Mins):** Look back with 20/20 hindsight. What design decisions were verified as correct, which ones created long-term technical debt, and how would they refactor it today?

---

## 📊 Background Discussion Rubric (Pass / Fail Metrics)

Evaluation focuses purely on depth of execution, operational accountability, and clarity of technical justification.

| Evaluation Pillar | Green Flags (Pass) | Red Flags (Fail) |
| :--- | :--- | :--- |
| **Systemic Ownership** | Speaks intimately and granularly about data models, background queues, API contracts, deployment barriers, and exact failure states of their past system. | Speaks strictly in generic abstractions, high-level buzzwords, or hand-waving; fails to explain the messy inner implementation details when pressed. |
| **Operational Transparency** | Openly and maturely details architectural mistakes, production outages, and poor trade-offs made in their past roles, providing a clear post-mortem analysis. | Frames all past projects as flawless architectures; minimizes engineering errors, hides system failures, or shifts blame away from their design choices. |
| **Technical Justification** | Explains past engineering choices using concrete operational metrics (e.g., team velocity, write throughput constraints, cloud budget) rather than personal aesthetic preferences. | Recommends frameworks, tools, or infrastructure dogmatically without tying choices to specific historical business or performance metrics. |

**Final Calculation:** To advance, the candidate must achieve a "Green Flag" across all three pillars.
