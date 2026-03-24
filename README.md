# The-Symbolic-Veto-An-ACT-R-Based-Architecture-for-Physical-Grounding-in-VLA-Robots

**Course:** Cognitive Architecture  
**Author:** Shubhkarman Singh and Avani Deshpande 

**Institution:** Dayananda Sagar University  

## 📌 Project Overview
Despite the rapid advancement of end-to-end Vision-Language-Action (VLA) models in robotic manipulation, these purely subsymbolic systems frequently hallucinate physical affordances. They often generate semantically plausible but physically impossible or unsafe motor commands (e.g., attempting to grasp a 2D picture of a mug).

This repository contains the literature review and foundational research for a hybrid neuro-symbolic architecture. By routing VLA predictions through a declarative cognitive buffer—inspired by the **ACT-R** framework—this architecture applies strict, symbolic physics constraints to systematically veto hallucinated actions prior to execution.

## 🗂️ Literature Survey Structure
This repository curates approximately 20 core research papers, categorized into three distinct domains necessary for building the Symbolic Veto architecture:

1. **The Limits of Vision-Language-Action (VLA) Models:** Establishing the baseline of current generative robotics and identifying the "semantic vs. physical reality" gap.
2. **Neuro-Symbolic Integration for Robotic Safety:** Exploring hybrid systems that combine the flexibility of neural networks with the deterministic safety of symbolic logic.
3. **Cognitive Architectures & LLM Integration:** Analyzing how established frameworks (like ACT-R) are being modernized to govern large language and vision models.

---

## 📚 Paper Reading List

### Area 1: Vision-Language-Action (VLA) Models & Limitations
| # | Title | Year | Key Takeaway / Relevance | Status |
|---|-------|------|--------------------------|--------|
| 1 | *[Paper Title Here]* | 202X | Defines baseline VLA capabilities and hallucination rates. | 📖 Reading |
| 2 | *[Paper Title Here]* | 202X | Addresses the brittleness of VLA physical grounding. | ⏳ Pending |
| 3 | *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 4 | *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 5 | *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 6 | *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |

### Area 2: Neuro-Symbolic Integration & Safety
| # | Title | Year | Key Takeaway / Relevance | Status |
|---|-------|------|--------------------------|--------|
| 7 | *[Paper Title Here]* | 202X | Explores the symbol grounding problem in modern ML. | ⏳ Pending |
| 8 | *[Paper Title Here]* | 202X | Uses symbolic constraints for scientific planning. | ⏳ Pending |
| 9 | *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 10| *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 11| *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 12| *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 13| *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |

### Area 3: Cognitive Architectures (ACT-R) governing LLMs
| # | Title | Year | Key Takeaway / Relevance | Status |
|---|-------|------|--------------------------|--------|
| 14| *[Paper Title Here]* | 202X | Introduces ACT-FLEX or similar ACT-R/LLM integrations. | ⏳ Pending |
| 15| *[Paper Title Here]* | 202X | Evaluates top-layer symbolic verifiers for neural outputs. | ⏳ Pending |
| 16| *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 17| *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 18| *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 19| *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |
| 20| *[Paper Title Here]* | 202X | *Summary of why this paper matters to the project.* | ⏳ Pending |

---

## 🛠️ Proposed Methodology (Next Steps)
1. **Literature Review:** Complete the reading list and synthesize the findings into a formal survey paper.
2. **Architecture Design:** Draft the data flow mapping a VLM's semantic output into an ACT-R working memory buffer.
3. **Procedural Logic:** Develop the declarative memory database (physical affordances) and the procedural production rules (IF/THEN veto triggers).
4. **Simulation (Future Scope):** Implement a proof-of-concept in a simulated environment to test the veto logic against forced VLA hallucinations.
