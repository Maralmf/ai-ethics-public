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

Measurement bias occurs when the variables used to represent real-world concepts systematically measure those concepts differently, inaccurately, or incompletely across individuals, groups, or contexts.

## Core Idea

AI systems rarely observe abstract concepts directly.

Instead, they rely on measurable proxies such as test scores, recorded diagnoses, income, click behaviour, arrest records, or performance evaluations.

If those measurements do not represent the underlying construct consistently, the model may learn distorted relationships.

## Why It Matters

A model can be statistically sophisticated and still be ethically problematic if the variables it uses do not measure the intended concepts equally well across populations.

Measurement bias can create or amplify disparities even when the dataset is otherwise representative.

## Mechanism

Measurement bias may arise when:

- the same underlying phenomenon is measured differently across groups
- measurement instruments have unequal validity
- administrative records capture some populations more completely than others
- access to measurement differs across groups
- subjective evaluations influence recorded variables
- observable variables are poor representations of latent concepts

## Example

Using recorded healthcare expenditure as a proxy for health need may underestimate the needs of populations that historically had less access to healthcare services.

Lower recorded spending does not necessarily imply lower medical need.

## Related Concepts

- [[0107 Proxy Bias]]
- [[0106 Label Bias]]
- [[Construct Validity]]
- [[Dataset Bias]]
- [[0109 Algorithmic Bias]]
- [[0120 Fairness]]

## Causes / Antecedents

- [[Poor Operationalization]]
- [[Unequal Access]]
- [[Institutional Practices]]
- [[Measurement Error]]
- [[Construct Underrepresentation]]

## Consequences

- [[Performance Disparity]]
- [[Group Harm]]
- [[0109 Algorithmic Bias]]
- [[Disparate Impact]]

## Mitigation / Controls

- [[Construct Validation]]
- [[Measurement Auditing]]
- [[Stakeholder Analysis]]
- [[Subgroup Analysis]]
- [[Alternative Measurement Design]]

## Measurement / Evaluation

Measurement bias can be evaluated by asking:

- Does the variable measure the intended construct?
- Is measurement quality comparable across groups?
- Are some groups systematically under-observed?
- Are administrative records shaped by unequal access or institutional practices?
- Does the measure have equivalent validity across contexts?

## Ethical Tensions

- [[Measurement Convenience vs Construct Validity]]
- [[Data Availability vs Fairness]]
- [[Standardization vs Context Sensitivity]]

## Key Sources

-

## Open Questions

- When is a proxy sufficiently valid to represent an ethical or social concept?
- How should measurement quality be assessed across demographic groups?
- Can standardized measurement itself create unfairness?