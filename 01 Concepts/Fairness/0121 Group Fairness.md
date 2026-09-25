---
type: concept
status:
  - developing
domains:
  - human-rights-justice
  - bias-fairness
aliases:
created: 2026-08-30
updated:
visibility: private
publish: false
---
## Definition

Group fairness evaluates whether an AI system produces sufficiently comparable treatment, outcomes, opportunities, or error patterns across socially relevant groups.

## Core Idea

Instead of asking whether every individual is treated fairly, group fairness compares aggregate outcomes across groups defined by characteristics such as:

- gender
- race or ethnicity
- age
- disability
- socioeconomic status
- other protected or relevant attributes

Different group fairness metrics formalize different notions of equality.

## Why It Matters

A system can perform well overall while systematically disadvantaging a subgroup.

Aggregate accuracy can therefore hide ethically important disparities.

## Common Operationalizations

- [[Demographic Parity]]
- [[Equal Opportunity]]
- [[Equalized Odds]]
- [[Predictive Parity]]
- [[Calibration]]

## Example

Suppose a credit model has:

- overall accuracy = 90%
- Group A false rejection rate = 8%
- Group B false rejection rate = 24%

Overall performance may appear strong, but the distribution of errors raises a group fairness concern.

## Related Concepts

- [[0120 Fairness]]
- [[0122 Individual Fairness]]
- [[Protected Attribute]]
- [[Subgroup Analysis]]
- [[0123 Intersectional Fairness]]
- [[Disparate Impact]]

## Causes / Antecedents

Group disparities may result from:

- [[Representation Bias]]
- [[Measurement Bias]]
- [[Historical Bias]]
- [[Label Bias]]
- [[Proxy Bias]]

## Consequences

- [[Group Harm]]
- [[0131 Discrimination]]
- [[Unequal Access]]
- [[Loss of Legitimacy]]

## Mitigation / Controls

- [[Fairness Auditing]]
- [[Subgroup Analysis]]
- [[Intersectional Analysis]]
- [[Bias Mitigation]]

## Measurement / Evaluation

Group fairness typically compares statistical quantities across groups, such as:

- selection rates
- true positive rates
- false positive rates
- false negative rates
- positive predictive values
- calibration

The ethical relevance of each metric depends on the decision context.

## Ethical Tensions

- [[0122 Individual Fairness]]
- [[0140 Fairness Metric Conflicts]]
- [[Fairness vs Performance]]
- [[Protected Attribute Use vs Fairness]]

## Key Sources

-

## Open Questions

- Which groups should be compared?
- How large can a disparity be before it becomes unacceptable?
- How should intersectional groups be handled?
- Can statistical equality conceal deeper structural injustice?