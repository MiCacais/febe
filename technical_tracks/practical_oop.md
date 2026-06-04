# 🧩 FeBe Technical Track: Practical Object-Oriented Programming (OOP)

**Best Suited For:** Mid-Level and Core Application Engineers
**Target Evaluation:** Domain modeling, state encapsulation, clean modular boundaries, and testable code architecture.

---

## 🚫 The Anti-Patterns to be aware of
* **No Academic Inheritance Riddles:** Do not evaluate deep, multi-tiered inheritance hierarchies (`Animal -> Mammal -> Dog`). Real-world application development heavily prefers composition, interfaces, and clear boundaries over complex type trees.
* **No Empty Whiteboards:** This track must be performed entirely inside a real IDE or shared development environment with syntax highlighting, auto-completion, and a testing framework initialized and operational from minute one.
* **No Syntax Gatekeeping:** Do not dock points because a candidate forgets the exact naming of a native collection method. Real engineers use documentation; allow them to look up syntax.

---

## 🛠️ The FeBe Alternative: The Domain Modeling Lab

Instead of an abstract riddle, provide the candidate with a clear business requirements doc and an empty or minimalist codebase with an active test suite. The task is to build out the structural logic for a self-contained system component.

### Example Problem Prompt:
> *"Design an in-memory shopping cart calculation engine that processes tiered discounts, caps maximum quantities based on user tiers, and calculates regional taxes based on item categories."*

### The Interview Structure (60 Minutes)
1. **The Context Brief (5 Mins):** Introduce the business domain, the input structures, the required outputs, and review the starter codebase setup.
2. **Domain Discovery (10 Mins):** The candidate walks through how they plan to model the data, define boundaries, and isolate internal state before writing any code.
3. **Hands-On Implementation (35 Mins):** The candidate implements the solution, utilizing standard unit tests to drive and verify their progress.
4. **The Constraints Pivot (10 Mins):** Introduce a sudden change in business requirements (e.g., *"What changes if a discount can now depend on an external, unpredictable coupon validation status?"*) to observe architectural flexibility and peer-to-peer engineering collaboration.

---

## 📊 Practical OOP Rubric (Pass / Fail Metrics)

Evaluation focuses purely on clean application discipline, state isolation, and maintainable structuring.

| Evaluation Pillar | Green Flags (Pass) | Red Flags (Fail) |
| :--- | :--- | :--- |
| **Domain Encapsulation** | Models data types and behaviors using clean, cohesive modules. Protects internal state configurations from leaking globally or being modified unsafely outside designated boundaries. | Writes monolithic, loose script structures with highly coupled modules. Exposes internal raw state to global, uncontrolled manipulation. |
| **Code Readability & Velocity** | Variable and method naming is explicit and intentional. The structural file layout is organized logically so a peer developer can easily navigate and modify the design. | Code layout is chaotic, single classes take on massive multi-purposed responsibilities (God objects), and internal logic flows are convoluted or overly dense. |
| **Testability & Design** | Code is constructed intentionally to allow simple unit testing boundaries. The candidate naturally writes clear assertions and keeps business logic decoupled from complex external framework setups. | The domain logic is tightly coupled to infrastructure or global states, making it impossible to isolate, verify, or unit test without writing extensive, fragile mock layers. |

**Final Calculation:** To advance, the candidate must achieve a "Green Flag" across all three pillars.
