---
type: concept
status:
  - developing
domains:
  - bias-fairness
  - ethical-tradeoffs
aliases:
created: 2026-08-30
updated:
visibility: private
publish: false
---
## Core Idea

Different fairness metrics formalize different normative ideas of fairness.

They therefore cannot be treated as interchangeable indicators of a single objective property.

In many realistic settings, multiple fairness criteria cannot be satisfied simultaneously.

## Core Conflict

Consider:

- [[Demographic Parity]]
- [[Equal Opportunity]]
- [[Equalized Odds]]
- [[Calibration]]
- [[Predictive Parity]]

Each asks a different question.

### Demographic Parity

Are positive decision rates equal?

### Equal Opportunity

Are qualified individuals equally likely to receive the positive decision?

### Equalized Odds

Are both true-positive and false-positive rates comparable?

### Calibration

Does the same score have the same empirical meaning across groups?

## Key Insight

A model can be fair according to one metric and unfair according to another.

Therefore:

> There is no context-independent fairness metric that universally determines whether an AI system is fair.

## Why Conflicts Occur

Fairness criteria condition on different quantities:

- predicted outcome
- actual outcome
- protected group
- risk score

When underlying outcome prevalence differs across groups, satisfying some combinations of fairness criteria may become mathematically incompatible except under special conditions.

## Ethical Implication

Selecting a fairness metric is therefore not merely a technical decision.

It requires normative judgment about:

- which harms matter
- which stakeholders should be protected
- which errors are most consequential
- whether equality of outcomes, opportunities, treatment, or reliability should be prioritized

## Related Concepts

- [[0120 Fairness]]
- [[0121 Group Fairness]]
- [[Fairness vs Performance]]
- [[Ethical Trade-offs]]
- [[Multi-Objective Ethics]]
- [[Stakeholder Analysis]]

## Open Questions

- Who should select the fairness criterion?
- Should affected communities participate in metric selection?
- How should conflicting fairness objectives be prioritized?
- Can several metrics be combined through multi-objective optimization?