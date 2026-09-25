---
type: concept
status:
  - developing
domains:
  - bias-fairness
  - harm-risk-power
aliases:
created: 2026-08-30
updated:
visibility: private
publish: false
---
## Definition

Algorithmic bias refers to systematic patterns in an algorithmic system that produce or contribute to unjustified differences in outcomes, treatment, errors, or opportunities across individuals or groups.

## Core Idea

Bias in an AI system does not necessarily originate inside the algorithm itself.

It may emerge from data, labels, measurements, feature design, objective functions, model assumptions, deployment conditions, or interactions between these elements.

Therefore, algorithmic bias should be understood as a system-level phenomenon rather than merely a mathematical defect in a model.

## Why It Matters

Algorithmic systems can scale decisions across large populations.

Small systematic disparities can therefore become widespread and persistent, particularly in high-stakes domains such as:

- hiring
- healthcare
- lending
- education
- criminal justice
- public services

## Mechanism

Algorithmic bias may emerge through:

- biased training data
- inappropriate target variables
- biased labels
- proxy variables
- unequal measurement quality
- optimization objectives that ignore subgroup effects
- inappropriate model assumptions
- distribution shift
- deployment in contexts different from the development environment
- feedback loops

## Example

A loan approval model may have high overall accuracy while producing a substantially higher false rejection rate for one demographic group.

The disparity may result from historical lending patterns, proxy variables, differences in data quality, or the model's optimization objective.

## Related Concepts

- [[0101 Historical Bias]]
- [[0102 Representation Bias]]
- [[0104 Sampling Bias]]
- [[0105 Measurement Bias]]
- [[0106 Label Bias]]
- [[0107 Proxy Bias]]
- [[0120 Fairness]]
- [[0131 Discrimination]]
- [[Disparate Impact]]

## Causes / Antecedents

- [[Dataset Bias]]
- [[0101 Historical Bias]]
- [[0105 Measurement Bias]]
- [[0106 Label Bias]]
- [[0107 Proxy Bias]]
- [[Objective Function]]
- [[0111 Deployment Bias]]

## Consequences

- [[Individual Harm]]
- [[Group Harm]]
- [[Disparate Impact]]
- [[Unequal Access]]
- [[0112 Feedback Loop Bias]]
- [[Loss of Trust]]

## Mitigation / Controls

- [[Fairness Auditing]]
- [[Bias Mitigation]]
- [[Dataset Auditing]]
- [[Subgroup Analysis]]
- [[Human Oversight]]
- [[Post-Deployment Monitoring]]

## Measurement / Evaluation

Algorithmic bias should generally be evaluated using multiple forms of evidence:

- subgroup performance metrics
- fairness metrics
- error-rate comparisons
- calibration analysis
- intersectional analysis
- qualitative stakeholder analysis
- evaluation of the decision context

No single metric can establish that an AI system is ethically unbiased.

## Ethical Tensions

- [[Fairness vs Performance]]
- [[0140 Fairness Metric Conflicts]]
- [[Privacy vs Fairness Auditing]]
- [[Individual Fairness vs Group Fairness]]

## Key Sources

-

## Open Questions

- When does a statistical disparity constitute ethically unacceptable bias?
- Should bias be assessed relative to historical reality or an ethical ideal?
- Can a model be unbiased while the overall decision system remains unfair?
- Who should determine acceptable levels of disparity?