---
type: concept
status:
  - developing
domains:
  - bias-fairness
aliases:
created: 2026-08-30
updated:
visibility: private
publish: false
---
## Definition

Sampling bias occurs when the process used to select observations for a dataset systematically produces a sample that differs from the population the AI system is intended to represent.

## Core Idea

Sampling bias concerns the mechanism by which observations enter the dataset.

If inclusion probabilities differ systematically across relevant groups or situations, the resulting dataset may provide a distorted picture of the target population.

## Why It Matters

Models generally learn patterns from the data they receive.

If the sampling process systematically excludes or overrepresents particular groups, locations, behaviours, or conditions, model outputs may be unreliable or unfair when deployed more broadly.

## Mechanism

Sampling bias can arise through:

- convenience sampling
- voluntary participation
- non-response
- geographic concentration
- platform-specific data collection
- institutional selection
- unequal probability of inclusion

## Example

A health prediction model trained only on patients from a large urban hospital may perform poorly when deployed in rural populations whose demographic, socioeconomic, or clinical characteristics differ substantially.

## Related Concepts

- [[0102 Representation Bias]]
- [[Selection Bias]]
- [[Dataset Bias]]
- [[External Validity]]
- [[Distribution Shift]]

## Causes / Antecedents

- [[Convenience Sampling]]
- [[Selection Mechanism]]
- [[Nonresponse Bias]]
- [[Data Availability]]

## Consequences

- [[0102 Representation Bias]]
- [[Performance Disparity]]
- [[0109 Algorithmic Bias]]
- [[Poor Generalization]]

## Mitigation / Controls

- [[Representative Sampling]]
- [[Stratified Sampling]]
- [[Sampling Weights]]
- [[Dataset Auditing]]
- [[External Validation]]

## Measurement / Evaluation

Sampling bias can be investigated by comparing the sample with the intended population and examining how observations were selected.

Evaluation may include:

- subgroup distributions
- sampling probabilities
- response rates
- geographic coverage
- comparison with external population statistics

## Ethical Tensions

- [[Data Quality vs Data Availability]]
- [[Fairness vs Cost]]
- [[Representation vs Privacy]]

## Key Sources

-

## Open Questions

- When does a non-representative sample become ethically unacceptable?
- How should sampling limitations be communicated to downstream users?
- Can reweighting adequately correct biased sampling processes?