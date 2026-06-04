# 🏡 FeBe Technical Track: Paid Take-Home Assessment Specification

**Best Suited For:** Application Engineers, Frontend/Backend Feature Developers, and Async-Preferred Candidates
**Target Evaluation:** Isolated execution capability, code organization, modular testability, and real-world production discipline.

---

## 🚫 The Anti-Patterns to be aware of
* **No Endless Homework Assignments:** If an assignment requires a candidate to burn a weekend, it is considered too lenthgy. The scope must be tailored to fit inside a 3-hour limit.
* **No Unpaid Exploitation:** If a company does not pay the mandatory **$150 to $200 flat-rate fee** for a completed submission, the pipeline is considered not FeBe friendly.
* **No Real Production Tasks:** Never ask a candidate to build actual features, refactor internal repositories, or squash active bugs for your corporate product. The project must exist entirely within a fictional, mocked domain.

---

## 🛠️ The FeBe Alternative: The Micro-Service Blueprint

Instead of providing a sweeping, vague prompt like *"Build a full-stack clone of our app,"* provide a highly localized, well-defined problem block. The project should ship with a pre-configured boilerplate repository containing an initialized test suite and basic environment files so the candidate doesn't waste their 3 hours wrestling with Webpack, Docker configs, or database connections. If the project needs deployment, this should also fit in the 2 - 3 hours timeline.

### Operational Scopes That Fit a 3-Hour Time Box:
* **Backend Focus:** Consuming a static JSON file of application server logs, processing the payload to find anomalous error spikes, and printing a structured summary report via a CLI utility.
* **Frontend Focus:** Building a responsive, accessible single-page layout that fetches data from a reliable, public mock API, implementing client-side filtering, and handling standard loading/error boundary states.

### The Execution Process
1. **The Contract Alignment:** Both parties sign the `take_home_agreement.md`, locking in the timeline, requirements, and the explicit flat fee payout.
2. **The 3-Hour Box:** The candidate executes on the repository asynchronously at a time of their choosing within the agreed multi-day submission window.
3. **The Simple Submission:** The candidate submits a link to their public/private repository or updates a zip file, alongside their standard payment invoice details.

---

## 🎯 Completion Boundaries & Non-Payment Recourse

To ensure mutual fairness, the framework enforces strict definitions on what constitutes a billable project, protecting companies from empty submissions and candidates from corporate ghosting.

### 1. The Definition of Completion
* **What Completion IS:** The candidate has implemented the baseline "happy path" requirements specified in the prompt, and the application boots up cleanly following the instructions in the `README.md`. Architectural imperfections, minor logical bugs, or missed edge cases do **not** invalidate completion; structural flaws will simply be reflected as a **Fail** on the interview scorecard, but the candidate's labor remains fully compensable.
* **The Kill-Fee Exception (Pro-Rated Dropouts):** If a candidate initiates work but realizes they are out of their depth, choose to withdraw from the hiring process, or abandon the assignment prior to baseline completion, they are entitled to a flat, pro-rated **$50 USD kill-fee** to compensate for their diagnostic setup time.

### 2. Safeguards Against Non-Payment
* **Conditional Evaluation License:** The candidate retains full copyright ownership of the code authored for the assignment. The company is granted a temporary license solely for internal evaluation. **This evaluation license is strictly conditional upon receipt of payment.**
* **Contract Breach Consequences:** If a company fails to process the flat-rate payment or kill-fee within **14 business days**, the evaluation license is automatically revoked. Continued corporate storage, usage, or review of the code constitutes an unauthorized breach. Furthermore, the candidate reserves the right to publicly report the non-paying organization to the open-source community non-compliance registry and hiring review platforms.

---

## 📊 Take-Home Project Rubric (Pass / Fail Metrics)

Evaluation must be performed objectively based on baseline code health and pragmatic trade-off analysis.

| Evaluation Pillar | Green Flags (Pass) | Red Flags (Fail) |
| :--- | :--- | :--- |
| **Correctness & Scope** | The application boots up cleanly following the README instructions and successfully executes the core baseline requirements specified in the prompt within the requested time box. | The code crashes on startup, fails to parse standard data inputs, or the candidate failed to complete the core assignment due to over-engineering out-of-scope features. |
| **Readability & Structure** | Variables are named intentionally, functions/classes are decoupled logically, and a peer developer can effortlessly navigate and reason about the codebase. | Massive monolithic code blocks, chaotic file layouts, or a complete lack of structural modularity that makes the solution unmaintainable. |
| **Pragmatic Discipline** | The submission includes basic error handling for obvious edge cases and provides a brief `README.md` explaining architectural trade-offs made due to the 3-hour limit. | The code panics on minor bad inputs, assumes a flawless runtime environment with zero error boundaries, or provides no documentation on decisions. |

**Final Calculation:** To advance, the candidate must achieve a "Green Flag" across all three pillars.
