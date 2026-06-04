# 🧮 FeBe Technical Track: Algorithmic Logic & Data Structures

**Best Suited For:** Fresh Grads, Junior Engineers, and Enterprise/Big Tech Organizations
**Target Evaluation:** Foundational logic processing, optimization reasoning, and code edge-case handling.

---

## 🚫 The Anti-Patterns to be aware of
* **No Brain-Teasers or Riddles:** Do not use trick problems that require a single "aha!" mathematical epiphany to solve. The question must rely on standard logic patterns, loops, and data structuring. 
* **No Syntax Penalties:** Do not reduce scores over missed semicolons or minor standard library naming discrepancies. Allow the use of documentation or Google throughout the evaluation.
* **No Hidden Test Cases:** Do not fail a candidate because their code didn't pass a hidden, unannounced boundary condition. If an edge case matters, state it clearly up front.

---

## 🛠️ The FeBe Alternative: The Open-Book Blueprint

If your pipeline utilizes this track, it is recommended to disclose the targeted concept domain to the candidate in their prep guide 5 days in advance. No hidden traps. It minimizes the risk of false positives and saves the candudate's time, so they know what to study and what not to focus on.

### Pre-Interview Disclosure Example:
> *"Our upcoming session will focus specifically on array manipulations and string parsing optimization. You will not need to memorize obscure tree-traversal algorithms or graph matrices."*

### The Interview Structure (60 Minutes)
1. **The Context Brief (5 Mins):** Present a clear problem statement with explicit inputs, expected outputs, and example test cases.
2. **The Logic Blueprint (15 Mins):** The candidate explains their conceptual approach *before* writing code. The interviewer validates boundaries to ensure no time is wasted on a misunderstood prompt.
3. **The Implementation (30 Mins):** The candidate builds out the functional solution inside a real IDE or shared text environment with syntax highlighting.
4. **The Optimizations & Trade-Offs (10 Mins):** Discuss time/space complexity ($O(n)$ metrics) and what compromises would be made under large scale.

---

## 📊 Algorithmic Logic Rubric (Pass / Fail Metrics)

Evaluation must be grounded strictly in logical translation and optimization reasoning.

| Evaluation Pillar | Green Flags (Pass) | Red Flags (Fail) |
| :--- | :--- | :--- |
| **Logical Execution** | Correctly translates a mental strategy into readable, working code that handles the base test data successfully. | Code features fundamental logic loops, infinite cycles, or a complete failure to translate conceptual pseudo-code into functional execution. |
| **Edge-Case Awareness** | Naturally accounts for boundary constraints (e.g., empty inputs, null pointers, array overflows) or fixes them gracefully when pointed out. | Code panics immediately on any variation of raw data; candidate fails to see major runtime vulnerabilities or acts defensively when an edge case is brought up. |
| **Optimization Clarity** | Understands the performance implications of their implementation and can confidently reason about time and space complexity ($O(n)$ metrics). | Demonstrates no awareness of code inefficiencies (e.g., nesting lookups blindly) or cannot reason about basic scaling trade-offs. |

**Final Calculation:** To advance, the candidate must achieve a "Green Flag" across all three pillars.
