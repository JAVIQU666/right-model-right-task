# Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI

Jiawei Qu, Kai Hou, Hongjie Jia, Jinyue Yan (2026). arXiv:2610.35189, v1 preprint. Submitted 26 October 2026; eess.SY.

[Original PDF](https://arxiv.org/pdf/2610.35189) · [arXiv record](https://arxiv.org/abs/2610.35189)

[Research questions and answers](QA.md) · [IEEE, Nature and Elsevier references](CITATIONS.md)

This Perspective proposes a framework for comparing the operational carbon emissions of generative-AI services at a specified level of task performance. Models would first need to meet explicit, task-specific capability requirements. Eligible models would then be compared by expected emissions per successfully completed task, accounting for failed attempts, retries and escalation as well as deployment-specific electricity carbon intensity. The paper illustrates the proposal with capability levels S1–S4 and carbon grades A–G, whose boundaries require future calibration. It also presents illustrative counterfactual scenarios for 2025 and projections to 2035. Under the assumed 2025 conditions, task-matched selection has estimated emissions of 16.9 Mt CO₂, compared with 47.0 Mt CO₂ for the reconstructed current-use baseline. These scenario estimates are not measured savings from an implemented labeling system. The authors identify standardized service assessments, comprehensive energy measurement, transparent carbon accounting and possible demand rebound as central implementation challenges.

## Key Findings

- The central proposal is to compare expected operational carbon emissions per successfully completed task at the required capability level. Task capability determines model eligibility before carbon performance is compared. ([PDF pp. 1–3, Abstract, Introduction, and Establishing Capability-constrained carbon labels; Fig. 1](https://arxiv.org/pdf/2610.35189#page=1))

- Both over-capability and under-capability can create inefficiency: excess computation may be unnecessary for routine tasks, while failures, retries and escalation can add energy costs when a model is insufficiently capable. This is the paper's conceptual rationale, rather than a new experimental benchmark of those mechanisms. ([PDF pp. 1–2, Introduction; Fig. 1a](https://arxiv.org/pdf/2610.35189#page=1))

- In the paper's illustrative 2025 scenarios, task-matched selection is estimated at 16.9 Mt CO₂, compared with 47.0 Mt CO₂ for a reconstructed current-use baseline: a reported 64.0% reduction under the assumed conditions. This is a counterfactual scenario estimate, not an observed reduction achieved by deployment. ([PDF pp. 4–5, Label-guided model selection and emissions; Fig. 3a](https://arxiv.org/pdf/2610.35189#page=4))

- The same illustrative 2025 comparison estimates 100.8 Mt CO₂ for capability-prioritized selection and 30.2 Mt CO₂ for energy-efficiency-prioritized selection. The comparison illustrates why model capability or energy efficiency alone may not identify the lowest-carbon successful service. ([PDF p. 5, Label-guided model selection and emissions; Fig. 3a](https://arxiv.org/pdf/2610.35189#page=5))

- The illustrative projection reports 61.6% lower emissions for task-matched selection relative to the reconstructed current-use baseline in 2035 under SSP5-8.5. Its magnitude depends on assumed task requirements, capability assessments, inference-energy data and future trajectories. ([PDF p. 5, Label-guided model selection and emissions; Fig. 3b](https://arxiv.org/pdf/2610.35189#page=5))

- Carbon labels should describe a model–task–deployment configuration, because electricity carbon intensity changes with location and time. The lowest-energy eligible model is therefore not necessarily the lowest-carbon eligible configuration. ([PDF p. 3, Establishing Capability-constrained carbon labels, third principle](https://arxiv.org/pdf/2610.35189#page=3))

## Methodology

- Study design: a Perspective presenting a proposed evaluation framework and an illustrative scenario analysis. The framework is organized around service-based comparability, comprehensive energy accounting and dynamic carbon accounting. ([PDF pp. 1–3, Abstract and Establishing Capability-constrained carbon labels](https://arxiv.org/pdf/2610.35189#page=1))

- Capability screening: define a task category and explicit performance or success thresholds, then assess whether each model meets the required capability level. Models exceeding the minimum requirement remain eligible and are compared against the same service requirement. ([PDF pp. 3–4, Establishing Capability-constrained carbon labels; Fig. 2](https://arxiv.org/pdf/2610.35189#page=3))

- Energy and carbon accounting: include failed attempts, repeated inference, retries and escalation in the energy required for successful completion; combine task-execution energy with serving-region and, where available, time-specific electricity carbon intensity. Report task definitions, hardware and inference settings consistently. ([PDF p. 3, Establishing Capability-constrained carbon labels, second and third principles](https://arxiv.org/pdf/2610.35189#page=3))

- Illustrative label design: S1–S4 represent increasing task-specific capability levels; eligible models receive carbon grades A–G based on expected operational emissions per successful task, with A lowest and G highest. The level boundaries and grade thresholds are illustrative and require calibration with standardized data. ([PDF pp. 3–4, Fig. 2 and Establishing Capability-constrained carbon labels](https://arxiv.org/pdf/2610.35189#page=3))

- Scenario construction: compare reconstructed current use, capability-prioritized selection, task-matched selection and energy-efficiency-prioritized selection. Published model-level token-use shares and benchmark-based capability classification provide a proxy for the baseline service-tier distribution. The energy-efficiency-prioritized scenario allows up to two attempts before escalation to a model meeting the required level. ([PDF pp. 4–5, Fig. 3 caption and Label-guided model selection and emissions](https://arxiv.org/pdf/2610.35189#page=4))

- Time horizon and uncertainty: estimate counterfactual operational emissions under 2025 conditions and explore 2025–2035 trajectories using IEA-informed assumptions about generative-AI growth and regional electricity carbon intensities under SSP1-2.6 and SSP5-8.5. Fig. 3a error bars reflect alternative capability-scoring systems, rather than a reported comprehensive uncertainty interval. ([PDF pp. 4–5, Fig. 3 caption and Label-guided model selection and emissions](https://arxiv.org/pdf/2610.35189#page=4))

## Limitations

- Author-stated: the magnitude of the scenario estimates depends on assumed task requirements, capability assessments and available inference-energy data. Reported percentages should be read within those assumptions. ([PDF p. 5, Label-guided model selection and emissions, final paragraph](https://arxiv.org/pdf/2610.35189#page=5))

- Explicit modeling assumption: token-use shares across capability levels are assumed to approximate the distribution of service requirements. The baseline therefore uses a proxy for task demand, not direct observation of each task's required capability. ([PDF pp. 4–5, Fig. 3 caption and Label-guided model selection and emissions](https://arxiv.org/pdf/2610.35189#page=4))

- Author-stated: capability-level boundaries and carbon-grade thresholds are illustrative rather than prescriptive. A usable label system would require calibration with standardized task-level performance, energy and carbon data. ([PDF p. 4, Establishing Capability-constrained carbon labels, final paragraph](https://arxiv.org/pdf/2610.35189#page=4))

- Author-stated: successful service is difficult to define for open-ended writing and complex reasoning. Evaluation may need multidimensional quality, reliability and safety criteria developed with domain experts, users and independent evaluators. ([PDF p. 6, Conclusion and outlook, first implementation priority](https://arxiv.org/pdf/2610.35189#page=6))

- Author-stated: consistent energy system boundaries and transparent reporting remain necessary; independent verification is particularly important for closed-weight models. Broader life-cycle impacts require improved evidence and reporting before incorporation. ([PDF p. 6, Conclusion and outlook, second and third implementation priorities](https://arxiv.org/pdf/2610.35189#page=6))

- Author-stated: lower emissions per successful task may not lower aggregate emissions if efficiency improvements stimulate additional demand. The proposal is a complement to cleaner electricity and more efficient computing. ([PDF p. 6, Conclusion and outlook, final paragraph](https://arxiv.org/pdf/2610.35189#page=6))

- Editorial interpretation of study scope: this Perspective and its illustrative scenarios do not establish real-world savings from an implemented labeling standard, a universal model ranking, or fixed eligibility thresholds suitable for every task. Those would require additional empirical evaluation and implementation evidence. ([Interpretation based on PDF pp. 1, 4–6: the paper identifies itself as a Perspective, makes its label thresholds illustrative, and describes future implementation requirements](https://arxiv.org/pdf/2610.35189#page=1))

## Abstract

The carbon footprint of generative-AI inference depends not only on hardware efficiency and electricity supply, but also on whether the selected model is appropriate for the task. A frontier model may expend unnecessary computation on a routine request, whereas an under-capable model may increase energy use through failure, retries, extended reasoning and escalation. However, a standardized evaluation framework that accounts for task-specific capability requirements and the carbon emissions associated with successful task remains lacking. In this Perspective, we argue for a capability-constrained carbon labeling framework that shifts environmental assessment from carbon intensity per inference towards the expected carbon emissions per successfully completed task at the required capability level. Under this framework, models would first be assessed against task-specific capability requirements, and only models capable of meeting those requirements would be compared on their expected energy use and operational carbon emissions. By linking service quality to carbon cost, this approach could enable more informed matching of the right model to the right task, offering a demand-side pathway to reducing emissions associated with generative-AI token use. Realizing this vision will require standardized capability-based service assessments, comprehensive energy accounting and transparent carbon disclosures.

## Research questions and answers

### What is capability-constrained carbon labeling for generative AI?

Capability-constrained carbon labeling compares expected operational emissions per successful task only among models that meet the task’s required performance. Source: Qu et al. (2026), arXiv:2610.35189; [PDF pp. 1–4, Abstract, Introduction, and Establishing Capability-constrained carbon labels; Figs. 1–2](https://arxiv.org/pdf/2610.35189#page=1). [Full answer](QA.md#q1).

### Why compare carbon emissions per successful AI task rather than per token or per query?

Emissions per successful task account for the service actually delivered, including failed attempts, retries and escalation that per-token or per-query measures may omit. Source: Qu et al. (2026), arXiv:2610.35189; [PDF pp. 1–3, Introduction and Establishing Capability-constrained carbon labels](https://arxiv.org/pdf/2610.35189#page=1). [Full answer](QA.md#q2).

### Is the smallest or most energy-efficient model always the lowest-carbon choice?

No. A smaller or lower-energy model can require retries or escalation, and electricity carbon intensity also affects the emissions of a successful service. Source: Qu et al. (2026), arXiv:2610.35189; [PDF pp. 1–3, Introduction and Establishing Capability-constrained carbon labels; PDF p. 5, illustrative scenario discussion](https://arxiv.org/pdf/2610.35189#page=1). [Full answer](QA.md#q3).

### What do the proposed S1–S4 capability levels and A–G carbon grades mean?

S1–S4 illustrate task-specific capability levels; A–G illustrate carbon grades among eligible models. The thresholds require calibration and are not a validated standard. Source: Qu et al. (2026), arXiv:2610.35189; [PDF pp. 3–4, Establishing Capability-constrained carbon labels; Fig. 2 and caption](https://arxiv.org/pdf/2610.35189#page=3). [Full answer](QA.md#q4).

### How much could task-matched model selection reduce generative-AI emissions?

The illustrative 2025 comparison reports 64.0% lower emissions for task-matched selection: 16.9 versus 47.0 Mt CO₂ for reconstructed current use. Source: Qu et al. (2026), arXiv:2610.35189; [PDF pp. 4–5, Label-guided model selection and emissions; Fig. 3 and caption](https://arxiv.org/pdf/2610.35189#page=4). [Full answer](QA.md#q5).

### How are the current-use and task-matched AI emissions scenarios constructed?

The study compares reconstructed current use with capability-prioritized, task-matched and energy-efficiency-prioritized selection using an illustrative scenario analysis. Source: Qu et al. (2026), arXiv:2610.35189; [PDF pp. 4–5, Fig. 3 caption and Label-guided model selection and emissions](https://arxiv.org/pdf/2610.35189#page=4). [Full answer](QA.md#q6).

### Why must an AI carbon label depend on where and when inference runs?

An AI carbon label depends on deployment because the same inference energy produces different emissions under different electricity carbon intensities across locations and times. Source: Qu et al. (2026), arXiv:2610.35189; [PDF p. 2, Introduction; PDF p. 3, Establishing Capability-constrained carbon labels, third principle; PDF p. 6, Conclusion and outlook](https://arxiv.org/pdf/2610.35189#page=2). [Full answer](QA.md#q7).

### Is capability-constrained carbon labeling a validated standard or a production routing system?

No. The paper proposes a framework and illustrative scenarios; it does not validate a complete labeling standard or a production routing service. Source: Qu et al. (2026), arXiv:2610.35189; [Study-scope interpretation based on PDF pp. 1, 4 and 6, Abstract, illustrative label design, and Conclusion and outlook](https://arxiv.org/pdf/2610.35189#page=1). [Full answer](QA.md#q8).

### Does capability-constrained carbon labeling cover the full AI life cycle?

No. The reported comparisons concern operational inference emissions; broader life-cycle impacts require further evidence and reporting. Source: Qu et al. (2026), arXiv:2610.35189; [PDF pp. 3–5, operational carbon accounting and scenario results; PDF p. 6, Conclusion and outlook, third implementation priority](https://arxiv.org/pdf/2610.35189#page=3). [Full answer](QA.md#q9).

### Would lower carbon emissions per successful task necessarily reduce total AI emissions?

No. Lower emissions per successful task can be offset by growth in demand, so per-task improvements do not alone establish lower aggregate AI emissions. Source: Qu et al. (2026), arXiv:2610.35189; [PDF p. 6, Conclusion and outlook, final paragraph](https://arxiv.org/pdf/2610.35189#page=6). [Full answer](QA.md#q10).

## How to cite this paper

### IEEE

J. Qu, K. Hou, H. Jia, and J. Yan, “Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI,” 2026, arXiv:2610.35189.

### Nature

Qu, J., Hou, K., Jia, H. & Yan, J. Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Preprint at https://arxiv.org/abs/2610.35189 (2026).

### Elsevier — numbered

J. Qu, K. Hou, H. Jia, J. Yan, Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI, arXiv preprint arXiv:2610.35189 (2026). https://arxiv.org/abs/2610.35189.

### Elsevier — author–year (Harvard)

Qu, J., Hou, K., Jia, H., Yan, J., 2026. Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. arXiv preprint arXiv:2610.35189. https://arxiv.org/abs/2610.35189.

[BibTeX](citation.bib) · [RIS](citation.ris) · [CSL-JSON](csl.json) · [Reference formats and style guidance](CITATIONS.md).
