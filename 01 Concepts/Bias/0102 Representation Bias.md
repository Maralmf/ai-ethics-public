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

Representation bias occurs when the data used to develop an AI system do not adequately represent the population, groups, environments, or situations in which the system will be used.

## Core Idea

A dataset may be large and technically well collected while still representing some populations substantially better than others.

The central issue is therefore not simply dataset size, but whether relevant variation in the target population is adequately represented.

## Why It Matters

Underrepresented groups may experience systematically poorer model performance, greater uncertainty, or more frequent errors.

Representation bias can therefore translate directly into unequal system quality across populations.

## Mechanism

Representation bias may arise because:

- some groups are difficult to recruit or observe
- data are collected from a narrow geographic or institutional context
- minority groups appear too infrequently in the dataset
- data collection channels systematically exclude certain populations
- the training population differs from the deployment population

## Example

A facial recognition model trained primarily on lighter-skinned faces may perform substantially worse on darker-skinned individuals because those populations were insufficiently represented during development.

## Related Concepts

- [[0104 Sampling Bias]]
- [[Selection Bias]]
- [[Dataset Bias]]
- [[Distribution Shift]]
- [[0121 Group Fairness]]
- [[0109 Algorithmic Bias]]

## Causes / Antecedents

- [[0104 Sampling Bias]]
- [[Selection Bias]]
- [[Data Availability]]
- [[Digital Divide]]

## Consequences

- [[Performance Disparity]]
- [[Group Harm]]
- [[False Positive Rate]]
- [[False Negative Rate]]
- [[0109 Algorithmic Bias]]

## Mitigation / Controls

- [[Representative Sampling]]
- [[Stratified Sampling]]
- [[Dataset Auditing]]
- [[Subgroup Analysis]]
- [[Data Augmentation]]

## Measurement / Evaluation

Representation can be evaluated by comparing the composition of the dataset with the intended target or deployment population.

Relevant analyses may include:

- subgroup frequencies
- coverage of relevant attributes
- intersectional representation
- comparison between training and deployment populations

## Ethical Tensions

- [[Representation vs Privacy]]
- [[Data Minimization vs Fairness]]
- [[Fairness vs Data Availability]]

## Key Sources

-

## Open Questions

- How much representation is sufficient for a minority subgroup?
- Should representation reflect the current population or deliberately compensate for historical exclusion?
- Which attributes should be considered when evaluating representativeness?