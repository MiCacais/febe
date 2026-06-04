# 🛠️ FeBe Technical Track Selection Matrix & Framework Rules

**Rule Number One:** Every FeBe-compliant hiring pipeline must select **ONE and only ONE** technical evaluation track. 

You cannot combine tracks. You cannot stack an architecture conversation on top of a coding challenge, nor can you follow an algorithm test with a system design loop. Identify the single most critical technical execution skill required for the role on Day 1, evaluate that exact capability, and respect the candidate's personal boundaries.

---

### 🎯 The "No Hidden Traps" Principle: Open-Book Focus Areas

Hiding the topic doesn't filter for deep engineering skills; it filters for luck. By broadcasting the exact focus areas, you eliminate the "lucky false positives" of candidates who happened to read a specific blog post or solve a matching puzzle the night before, while giving every builder a fair chance to show how they execute within a known domain.

**What this looks like in practice across FeBe tracks:**
* **If it's Algorithmic Logic:** Specify the exact data domain (e.g., *"We will focus on array manipulation and string parsing optimization."*)
* **If it's Core Domain Trivia / Code Review:** Specify the exact runtime paradigms (e.g., *"We will be reviewing a legacy Pull Request with a heavy focus on debugging async/await concurrency and handling race conditions."*)
* **If it's System Design:** Specify the architectural pattern and infrastructure components (e.g., *"We will be evaluating system evolution with a strict focus on event-driven design, SQS message queuing, and handling dead-letter queues."*)
* **If it's Practical OOP:** Specify the structural boundaries (e.g., *"We will be evaluating clean domain modeling with a focus on state encapsulation and decoupling logic from external databases."*)
* **If it's a Background Architecture Discussion:** Specify the system characteristics to review (e.g., *"We will be diving deep into the most complex production system you've shipped, specifically focusing on how you managed database connection pooling and multi-region data replication under load."*)

---

## 📊 FeBe Selection Matrix & Recommendations

To maximize pipeline efficiency, the single technical track chosen must match both the organizational reality of your company and the seniority level of the target engineering profile.

| Company Stage | Junior / Fresh Grad | Mid-Level / Core Engineer | Senior / Staff Architect |
| :--- | :--- | :--- | :--- |
| **Early Startup / Seed to Series A** | Algorithmic Logic *or* Paid Take-Home | Core Domain Trivia *or* Practical OOP | System Design *or* Background Discussion |
| **Growth Scale-Up / Series B+** | Algorithmic Logic (w/ Prep Guide) | Practical OOP *or* Paid Take-Home | System Design *or* Background Discussion |
| **Enterprise / Mature Big Tech** | **Algorithmic Logic** (Recommended) | Core Domain Trivia *or* Practical OOP | System Design *or* Background Discussion |

---

## 💡 Strategic Recommendations & Core Alignment

### 🎓 The Algorithm / Data Structures (DS) Exception
FeBe recommends abstract algorithmic testing (LeetCode-style) strictly for two specific use cases:
1. **Fresh Grads & Entry-Level Talent:** Candidates lacking extensive production code histories cannot easily be evaluated on legacy code review or system maintenance. Algorithmic logic serves as a baseline for foundational processing.
2. **Enterprise & Mature "Big Tech" Ecosystems:** Organizations handling massive global scaling infrastructure where core data structures, memory constraints, and algorithmic optimizations directly impact day-to-day delivery.

### 🔍 Keeping the Tracks Fragmented and Non-Negotiable
To prevent interview loops from bleeding into one another, every track must remain isolated and independent:
* **Background Architecture Discussion:** A retrospective review of a complex project the candidate *actually built* in their career.
* **Core Domain Trivia & Code Review:** An exercise evaluating code comprehension, optimization, and collaboration using a pre-written Pull Request.
* **Practical OOP:** A coding track assessing clean modular boundaries, domain modeling, and state isolation.
* **System Design:** An evolutionary analysis of system scalability, operational bottlenecks, and infrastructure trade-offs.
* **Take-Home Assessment:** A 2-to-3-hour maximum, fully compensated operational programming assignment.
