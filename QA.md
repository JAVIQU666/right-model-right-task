# Research Q&A: Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI

Jiawei Qu; Kai Hou; Hongjie Jia; Jinyue Yan. 2026. arXiv:2610.35189, v1 preprint.

<a id="q1"></a>

## What is capability-constrained carbon labeling for generative AI?

**Direct answer:** Capability-constrained carbon labeling compares expected operational emissions per successful task only among models that meet the task’s required performance.

**Explanation:** It is a proposed way to compare the operational carbon cost of AI services at a defined level of performance. First, models must meet the task's explicit capability requirements. Only eligible models are then compared by expected emissions per successfully completed task. The accounting should include failures, retries and escalation, together with the electricity carbon intensity of deployment. The paper presents this as a Perspective framework that still requires standardized assessments and calibration.

**Source paper:** Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Qu et al. (2026), arXiv:2610.35189, v1.

**Evidence:** [PDF pp. 1–4, Abstract, Introduction, and Establishing Capability-constrained carbon labels; Figs. 1–2](https://arxiv.org/pdf/2610.35189#page=1).

<a id="q2"></a>

## Why compare carbon emissions per successful AI task rather than per token or per query?

**Direct answer:** Emissions per successful task account for the service actually delivered, including failed attempts, retries and escalation that per-token or per-query measures may omit.

**Explanation:** A single query can consume little energy yet fail to deliver the service the user needs. Repeating the request, generating additional reasoning or escalating to another model adds energy before a successful result is obtained. The paper therefore argues that comparisons should capture the expected carbon cost of delivering a successful task at a specified quality level. Per-token and per-query measurements alone may omit these additional attempts and do not establish equivalent service quality.

**Source paper:** Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Qu et al. (2026), arXiv:2610.35189, v1.

**Evidence:** [PDF pp. 1–3, Introduction and Establishing Capability-constrained carbon labels](https://arxiv.org/pdf/2610.35189#page=1).

<a id="q3"></a>

## Is the smallest or most energy-efficient model always the lowest-carbon choice?

**Direct answer:** No. A smaller or lower-energy model can require retries or escalation, and electricity carbon intensity also affects the emissions of a successful service.

**Explanation:** No universal rule of that kind is supported by this paper. A smaller or efficient model may be suitable when it reliably meets the task requirements. If it fails and triggers retries or escalation, the total energy needed for successful completion may rise. Carbon emissions also depend on the electricity supplying inference. The proposed decision rule is to identify eligible models first, then compare expected operational emissions for the task and deployment configuration.

**Source paper:** Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Qu et al. (2026), arXiv:2610.35189, v1.

**Evidence:** [PDF pp. 1–3, Introduction and Establishing Capability-constrained carbon labels; PDF p. 5, illustrative scenario discussion](https://arxiv.org/pdf/2610.35189#page=1).

<a id="q4"></a>

## What do the proposed S1–S4 capability levels and A–G carbon grades mean?

**Direct answer:** S1–S4 illustrate task-specific capability levels; A–G illustrate carbon grades among eligible models. The thresholds require calibration and are not a validated standard.

**Explanation:** S1–S4 illustrate increasing capability levels within a task category, such as coding, writing or mathematical reasoning. A model must meet or exceed the requested level to be eligible. Eligible models are then compared using A–G grades for expected operational emissions per successful task, with A representing the lowest emissions and G the highest. These are illustrative labels: the paper does not establish final standardized performance thresholds or carbon-grade boundaries.

**Source paper:** Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Qu et al. (2026), arXiv:2610.35189, v1.

**Evidence:** [PDF pp. 3–4, Establishing Capability-constrained carbon labels; Fig. 2 and caption](https://arxiv.org/pdf/2610.35189#page=3).

<a id="q5"></a>

## How much could task-matched model selection reduce generative-AI emissions?

**Direct answer:** The illustrative 2025 comparison reports 64.0% lower emissions for task-matched selection: 16.9 versus 47.0 Mt CO₂ for reconstructed current use.

**Explanation:** Under the paper's assumed 2025 conditions, task-matched selection is estimated at 16.9 Mt CO₂ versus 47.0 Mt CO₂ for reconstructed current use, a reported 64.0% reduction. The illustrative 2035 SSP5-8.5 pathway reports 61.6% lower emissions relative to that baseline. These are counterfactual and projected scenario results, not measured deployment savings. Their magnitudes depend on task-demand assumptions, capability assessments, inference-energy inputs and future trajectories, so they should not be treated as guaranteed reductions.

**Source paper:** Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Qu et al. (2026), arXiv:2610.35189, v1.

**Evidence:** [PDF pp. 4–5, Label-guided model selection and emissions; Fig. 3 and caption](https://arxiv.org/pdf/2610.35189#page=4).

<a id="q6"></a>

## How are the current-use and task-matched AI emissions scenarios constructed?

**Direct answer:** The study compares reconstructed current use with capability-prioritized, task-matched and energy-efficiency-prioritized selection using an illustrative scenario analysis.

**Explanation:** The paper compares reconstructed current use with capability-prioritized, task-matched and energy-efficiency-prioritized selection. Published model-level token-use shares, classified using benchmark scores, serve as a proxy for the distribution of required service levels. The energy-efficiency-prioritized scenario allows up to two attempts before escalation. The authors estimate 2025 counterfactual emissions and explore trajectories to 2035 using IEA-informed growth assumptions and electricity carbon intensities under SSP1-2.6 and SSP5-8.5. This is illustrative scenario analysis, rather than a new live-routing trial.

**Source paper:** Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Qu et al. (2026), arXiv:2610.35189, v1.

**Evidence:** [PDF pp. 4–5, Fig. 3 caption and Label-guided model selection and emissions](https://arxiv.org/pdf/2610.35189#page=4).

<a id="q7"></a>

## Why must an AI carbon label depend on where and when inference runs?

**Direct answer:** An AI carbon label depends on deployment because the same inference energy produces different emissions under different electricity carbon intensities across locations and times.

**Explanation:** The same amount of task-execution energy can produce different operational emissions when electricity carbon intensity differs across regions or times. The paper therefore proposes combining energy per successful task with serving-region and, where available, time-specific carbon intensity. A label would describe a model–task–deployment configuration and need updates as conditions change. Carbon-aware routing could use this information where latency, privacy and availability constraints allow, rather than assuming a model has one permanent carbon grade.

**Source paper:** Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Qu et al. (2026), arXiv:2610.35189, v1.

**Evidence:** [PDF p. 2, Introduction; PDF p. 3, Establishing Capability-constrained carbon labels, third principle; PDF p. 6, Conclusion and outlook](https://arxiv.org/pdf/2610.35189#page=2).

<a id="q8"></a>

## Is capability-constrained carbon labeling a validated standard or a production routing system?

**Direct answer:** No. The paper proposes a framework and illustrative scenarios; it does not validate a complete labeling standard or a production routing service.

**Explanation:** The paper proposes a framework and illustrates its implications; it does not report implementation and validation of a complete labeling standard or production routing service. Its capability levels and carbon-grade thresholds require calibration. The outlook calls for shared evaluation protocols, comprehensive energy measurements, transparent deployment-specific carbon accounting and independent verification. The paper can guide the design of future evaluations, but its illustrative labels should not be presented as certified grades for named commercial models.

**Source paper:** Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Qu et al. (2026), arXiv:2610.35189, v1.

**Evidence:** [Study-scope interpretation based on PDF pp. 1, 4 and 6, Abstract, illustrative label design, and Conclusion and outlook](https://arxiv.org/pdf/2610.35189#page=1).

<a id="q9"></a>

## Does capability-constrained carbon labeling cover the full AI life cycle?

**Direct answer:** No. The reported comparisons concern operational inference emissions; broader life-cycle impacts require further evidence and reporting.

**Explanation:** The proposed comparisons and illustrative results focus on operational emissions associated with inference and successful task completion. The paper discusses translating task-level energy into emissions using the electricity supplying inference. It also states that broader life-cycle impacts should be incorporated as evidence and reporting improve. Accordingly, the reported scenario totals should not be described as a complete life-cycle assessment covering all training, hardware manufacture, infrastructure construction and other upstream or downstream impacts.

**Source paper:** Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Qu et al. (2026), arXiv:2610.35189, v1.

**Evidence:** [PDF pp. 3–5, operational carbon accounting and scenario results; PDF p. 6, Conclusion and outlook, third implementation priority](https://arxiv.org/pdf/2610.35189#page=3).

<a id="q10"></a>

## Would lower carbon emissions per successful task necessarily reduce total AI emissions?

**Direct answer:** No. Lower emissions per successful task can be offset by growth in demand, so per-task improvements do not alone establish lower aggregate AI emissions.

**Explanation:** No. The authors explicitly note that efficiency gains may stimulate additional demand, so lower emissions per successful task may not reduce aggregate emissions. The proposed labels address the carbon cost of delivering a defined service; total emissions also depend on how much service is consumed. The paper frames capability-constrained labeling as a demand-side complement to cleaner electricity and more efficient computing, not as a standalone guarantee of falling sector-wide emissions.

**Source paper:** Right Model, Right Task: Capability-Constrained Carbon Labeling to Decarbonize Generative AI. Qu et al. (2026), arXiv:2610.35189, v1.

**Evidence:** [PDF p. 6, Conclusion and outlook, final paragraph](https://arxiv.org/pdf/2610.35189#page=6).

## Reference formats

[IEEE, Nature and Elsevier](CITATIONS.md) · [BibTeX](citation.bib) · [RIS](citation.ris).
