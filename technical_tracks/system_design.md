# 🏛️ FeBe Technical Track: Practical System Design Spec

**Best Suited For:** Senior, Staff, and Principal Engineers
**Target Evaluation:** Trade-off analysis, architectural maintenance realities, and production pragmatism.

---

## 🚫 The Anti-Patterns to be aware of
* **Do not use hyper-scale hypotheticals:** Unless you are genuinely operating at the scale of Netflix or Twitter, do not ask a candidate to "Design Twitter from scratch." It forces candidates to regurgitate memorized buzzwords (e.g., "Kafka," "Redis Caching") rather than solving real problems.
* **Do not grade on presentation slickness:** An engineer who draws a beautifully balanced diagram but fails to understand database lock contention is an interview performer. An engineer with messy whiteboard boxes who perfectly describes replication lag is an executioner.
* **No Infinite Budgets:** Do not let candidates design systems assuming infinite compute resources, zero latency cost, or unlimited engineering velocity. 

---

## 🛠️ The FeBe Alternative: The "Evolutionary" Architecture Review

Instead of an abstract, blank-canvas design prompt, provide the candidate with a basic, messy, architecture diagram of a system that resembles your company's actual domain 1 to 2 years ago. 

### Pre-Interview Disclosure Example:
As mandated by the "No Hidden Traps" principle, the interviewer must specify the architectural focus at least 5 business days in advance:
> *"We will be evaluating system evolution with a strict focus on event-driven design, SQS message queuing, and handling dead-letter queues."*

### The Prompt Structure:
1. **The Baseline:** *"Here is a high-level overview of our core monolith and database architecture from two years ago. It worked perfectly when we had 10,000 users."*
2. **The Problem:** *"We are now scaling past 500,000 users, and we are experiencing severe performance degradation on [Specific Endpoint] and database connection exhaustion. Walk us through how you would diagnose, isolate, and systematically evolve this architecture to handle the load."*

### The Interview Structure (60 Minutes)
1. **The Infrastructure Briefing (10 Mins):** Introduce the legacy diagram, baseline traffic data, and data flow constraints. 
2. **Bottleneck Identification (15 Mins):** The candidate forensicly analyzes the legacy map, pointing out immediate points of failure under the new load targets.
3. **Systemic Evolution (25 Mins):** The candidate modifies the architecture map live, introducing decoupling components, queuing strategies, or data store alternatives to resolve the bottlenecks.
4. **The Reality Check (10 Mins):** The interviewer introduces a practical production constraint (e.g., *"Our main cloud provider drops connectivity to our message broker for 45 seconds. How does this evolved setup survive?"*).

---

## 📊 Objective System Design Rubric (Pass / Fail Metrics)

Evaluation must be grounded strictly in engineering execution and trade-off analysis.

| Evaluation Pillar | Green Flags (Pass) | Red Flags (Fail) |
| :--- | :--- | :--- |
| **Trade-Off Awareness** | Explicitly states what is being sacrificed when choosing a technology (e.g., *"Adding an SQS queue handles asynchronous spikes, but introduces data eventual consistency issues we have to handle in the UI"*). | Recommends technologies dogmatically without acknowledging their structural downsides, operational complexity, or infrastructure costs. |
| **Pragmatic Scaling** | Focuses on systemic bottlenecks first (e.g., database indexing, query optimization, horizontal scaling) before leaping to complex microservices architectures. | Instantly jumps to over-engineered, complex distributed systems for a problem that could be solved with a simple database replica or localized cache. |
| **Collaborative Communication** | Treats the interviewer as a peer engineering partner, validating assumptions and checking boundaries before making sweeping structural decisions. | Delivers a one-way, unyielding lecture or acts defensively when alternative infrastructure solutions are suggested. |

**Final Calculation:** To advance, the candidate must achieve a "Green Flag" across all three core evaluation pillars.
