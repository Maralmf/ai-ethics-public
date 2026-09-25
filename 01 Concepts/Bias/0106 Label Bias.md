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

Label bias occurs when the target labels used to train or evaluate an AI system systematically reflect subjective judgments, inconsistent standards, institutional practices, or biased historical decisions rather than the intended underlying outcome.

## Core Idea

Supervised learning assumes that training labels represent the ground truth.

In many socially consequential domains, however, labels are not objective facts.

They may reflect human judgments, institutional decisions, incomplete observations, or historically biased processes.

## Why It Matters

If biased labels are treated as ground truth, an AI system can reproduce those judgments at scale while giving them the appearance of statistical objectivity.

## Mechanism

Label bias may arise through:

- subjective human annotation
- inconsistent labeling criteria
- historical decision-making
- institutional discrimination
- incomplete outcome observation
- labels that capture decisions rather than underlying reality

## Example

A model predicting employee "success" may be trained using past promotion decisions as the target label.

If promotion decisions were historically influenced by gender or racial bias, the target label itself may encode discrimination.

## Related Concepts

- [[0101 Historical Bias]]
- [[0105 Measurement Bias]]
- [[Annotation Bias]]
- [[Ground Truth]]
- [[0109 Algorithmic Bias]]
- [[Human Judgment]]

## Causes / Antecedents

- [[Subjective Evaluation]]
- [[Historical Discrimination]]
- [[Inconsistent Standards]]
- [[Institutional Bias]]
- [[Annotation Bias]]

## Consequences

- [[0109 Algorithmic Bias]]
- [[Disparate Impact]]
- [[0112 Feedback Loop Bias]]
- [[Group Harm]]

## Mitigation / Controls

- [[Label Auditing]]
- [[Multiple Annotators]]
- [[Inter-Rater Reliability]]
- [[Alternative Outcome Definition]]
- [[Stakeholder Review]]

## Measurement / Evaluation

Label bias can be investigated by examining:

- who created the labels
- how labeling criteria were defined
- whether criteria were applied consistently
- whether disagreement exists between annotators
- whether labels reflect outcomes, decisions, or judgments
- whether label quality varies across groups

## Ethical Tensions

- [[Human Judgment vs Statistical Consistency]]
- [[Historical Labels vs Normative Ground Truth]]
- [[Efficiency vs Label Quality]]

## Key Sources

-

## Open Questions

- When can a historical decision legitimately be used as a training label?
- Who should define the ground truth in socially contested domains?
- How should disagreement between expert annotators be represented?