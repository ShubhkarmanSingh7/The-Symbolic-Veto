# The Symbolic Veto: An ACT-R Based Architecture for Physical Grounding in VLA Robots

**Course:** Cognitive Architecture  
**Author:** Shubhkarman Singh, Avani Deshpande, Rutu Patil**Institution:** Dayananda Sagar University

## 📌 Project Overview

Despite the rapid advancement of end-to-end Vision-Language-Action (VLA) models in robotic manipulation, these purely subsymbolic systems frequently hallucinate physical affordances. They often generate semantically plausible but physically impossible or unsafe motor commands (e.g., attempting to grasp a 2D picture of a mug).

This repository contains the literature review and foundational research for a hybrid neuro-symbolic architecture. By routing VLA predictions through a declarative cognitive buffer—inspired by the **ACT-R** framework—this architecture applies strict, symbolic physics constraints to systematically veto hallucinated actions prior to execution.

## 🗂️ Literature Survey Structure

This repository curates 20 core research papers (all published 2023–2026), categorized into three distinct domains necessary for building the Symbolic Veto architecture:

1. **The Limits of Vision-Language-Action (VLA) Models:** Establishing the baseline of current generative robotics and identifying the "semantic vs. physical reality" gap.
2. **Neuro-Symbolic Integration for Robotic Safety:** Exploring hybrid systems that combine the flexibility of neural networks with the deterministic safety of symbolic logic.
3. **Cognitive Architectures & LLM Integration:** Analyzing how established frameworks (like ACT-R) are being modernized to govern large language and vision models.

* * *

## 📚 Paper Reading List

### Area 1: Vision-Language-Action (VLA) Models & Limitations

| # | Title | Authors | Year | Key Takeaway / Relevance | 
|---|-------|---------|------|--------------------------|
| 1 | [RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818) | Brohan et al. (CoRL) | 2023 | Coins "VLA" and defines the baseline: actions as text tokens from a web-pretrained VLM. |
| 2 | [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) | Kim et al. | 2024 | Open, reproducible VLA; a realistic target model for the veto layer in simulation. |
| 3 | [π0: A Vision-Language-Action Flow Model for General Robot Control](https://arxiv.org/abs/2410.24164) | Black et al. (Physical Intelligence) | 2024 | State-of-the-art generalist policy using flow matching; shows what the veto must sit on top of. | 
| 4 | [A Survey on Vision-Language-Action Models for Embodied AI](https://arxiv.org/abs/2405.14093) | Ma et al. | 2024 | Taxonomy of VLAs (components, control policies, task planners) and open challenges. | 
| 5 | [Towards Testing and Evaluating Vision-Language-Action Models for Robotic Manipulation: An Empirical Study (VLATest)](https://arxiv.org/abs/2409.12894) | Wang et al. (FSE 2025) | 2024 | Fuzzing-based testing of 7 VLA models; empirical evidence of brittleness under scene variation. | 
| 6 | [Exploring the Adversarial Vulnerabilities of Vision-Language-Action Models in Robotics](https://arxiv.org/abs/2411.13587) | Wang et al. (ICCV 2025) | 2024 | Adversarial patches and attacks that cause VLA task failure, motivating an independent safety check. | 

### Area 2: Neuro-Symbolic Integration & Safety

| # | Title | Authors | Year | Key Takeaway / Relevance | 
|---|-------|---------|------|--------------------------|
| 7 | [Neurosymbolic Grounding for Compositional World Models (Cosmos)](https://arxiv.org/abs/2310.12690) | Sehgal et al. (ICLR 2024) | 2023 | Symbol grounding in modern ML: vision-language models assign symbolic attributes to entities. | 
| 8 | [LLM+P: Empowering Large Language Models with Optimal Planning Proficiency](https://arxiv.org/abs/2304.11477) | Liu et al. | 2023 | LLM translates the task and a classical symbolic planner guarantees plan validity. | 
| 9 | [Logic-LM: Empowering Large Language Models with Symbolic Solvers for Faithful Logical Reasoning](https://arxiv.org/abs/2305.12295) | Pan et al. | 2023 | Symbolic solver verifies and corrects neural reasoning output. | 
| 10 | [AutoTAMP: Autoregressive Task and Motion Planning with LLMs as Translators and Checkers](https://arxiv.org/abs/2306.06531) | Chen et al. | 2023 | LLM output is formally checked against constraints before execution. | 
| 11 | [Jailbreaking LLM-Controlled Robots (RoboPAIR)](https://arxiv.org/abs/2410.13691) | Robey et al. | 2024 | Shows neural-only safety fails when an LLM drives a physical robot. | ⏳ Pending |
| 12 | [Safety Guardrails for LLM-Enabled Robots (RoboGuard)](https://arxiv.org/abs/2503.07885) | Ravichandran et al. (RA-L 2026) | 2025 | Closest prior work to the veto idea: temporal-logic control synthesis over LLM plans. Position against it. | 
| 13 | [Neuro-Symbolic AI in 2024: A Systematic Review](https://arxiv.org/abs/2501.05435) | Colelough & Regli | 2025 | PRISMA survey of the field; anchors the neuro-symbolic framing and open gaps. | 

### Area 3: Cognitive Architectures (ACT-R) governing LLMs

| # | Title | Authors | Year | Key Takeaway / Relevance | 
|---|-------|---------|------|--------------------------|
| 14 | [Cognitive LLMs: Towards Integrating Cognitive Architectures and Large Language Models for Manufacturing Decision-making (LLM-ACTR)](https://arxiv.org/abs/2408.09176) | Wu, Oltramari, Francis, Giles, Ritter | 2024 | Direct ACT-R + LLM integration (ACT-R knowledge injected into LLM adapters). Opposite direction to the veto: a useful contrast. |
| 15 | [LLM-ACTR: from Cognitive Models to LLMs in Manufacturing Solutions](https://doi.org/10.1609/aaaiss.v5i1.35610) | Wu et al. (AAAI Symposium Series) | 2025 | Follow-up framing ACT-R as a remedy for insufficient grounding in LLMs. |
| 16 | [Enabling High-Level Machine Reasoning with Cognitive Neuro-Symbolic Systems](https://ojs.aaai.org/index.php/AAAI-SS/article/view/27701) | Oltramari (AAAI Symposium Series) | 2023 | Hybrid framework centered on ACT-R plus generative models for commonsense reasoning. | 
| 17 | [ACT-R model monitoring an LLM-driven robot dialog (BAILAR workshop, paper 1)](https://ceur-ws.org/Vol-3906/paper1_BAILAR.pdf) | BAILAR 2024 authors (CEUR-WS Vol. 3906) | 2024 | ACT-R supervises LLM output on a robot and intervenes when needed: nearest precedent to the veto. | 
| 18 | [Cognitive Architectures for Language Agents (CoALA)](https://arxiv.org/abs/2309.02427) | Sumers et al. (TMLR) | 2023 | Standard framework mapping memory and decision modules onto LLM agents. | 
| 19 | [Applying Cognitive Design Patterns to General LLM Agents](https://arxiv.org/abs/2505.07087) | Wray, Kirk, Laird (AGI 2025) | 2025 | Argues recurring cognitive-architecture patterns explain and fix LLM-agent gaps. (arXiv v1 title: *Architectural Precedents for General Agents using Large Language Models*.) |
| 20 | [Exploiting Language Models as a Source of Knowledge for Cognitive Agents](https://arxiv.org/abs/2310.06846) | Kirk, Wray, Laird (AAAI FSS 2023) | 2023 | Soar-based, but the LLM-to-symbolic-memory interface is directly relevant to the declarative buffer. | 

* * *

## 🛠️ Proposed Methodology (Next Steps)

1. **Literature Review:** Complete the reading list and synthesize the findings into a formal survey paper.
2. **Architecture Design:** Draft the data flow mapping a VLM's semantic output into an ACT-R working memory buffer.
3. **Procedural Logic:** Develop the declarative memory database (physical affordances) and the procedural production rules (IF/THEN veto triggers).
4. **Simulation (Future Scope):** Implement a proof-of-concept in a simulated environment to test the veto logic against forced VLA hallucinations.
