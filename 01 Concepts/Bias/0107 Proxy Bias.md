---
type: concept
status:
  - developing
domains:
  - bias-fairness
  - privacy-data-governance
aliases:
created: 2026-08-30
updated:
visibility: private
publish: false
---
## Definition

Proxy bias occurs when a variable that appears neutral functions as a substitute for a sensitive, protected, or socially meaningful characteristic and thereby reproduces disparities associated with that characteristic.

## Core Idea

Removing a protected attribute from a dataset does not necessarily remove its influence.

Other variables may encode similar information and allow a model to reconstruct or approximate the protected characteristic indirectly.

## Why It Matters

A system may appear formally "blind" to race, gender, socioeconomic status, or other protected attributes while still producing decisions strongly shaped by correlated proxy variables.

This makes fairness-by-unawareness an unreliable strategy.

## Mechanism

Proxy bias may arise when variables such as:

- postal code
- school attended
- employment history
- language
- purchasing patterns
- device type
- neighbourhood characteristics

are strongly correlated with protected or sensitive attributes.

## Example

A credit model that excludes race but heavily relies on postal code may indirectly reproduce racial disparities if residential geography is strongly shaped by historical segregation.

## Related Concepts

- [[Protected Attribute]]
- [[Sensitive Attribute]]
- [[Fairness Through Unawareness]]
- [[0105 Measurement Bias]]
- [[0109 Algorithmic Bias]]
- [[Indirect Discrimination]]

## Causes / Antecedents

- [[Feature Correlation]]
- [[Historical Segregation]]
- [[Structural Inequality]]
- [[Feature Engineering]]

## Consequences

- [[Indirect Discrimination]]
- [[Disparate Impact]]
- [[Group Harm]]
- [[Privacy Risk]]

## Mitigation / Controls

- [[Proxy Detection]]
- [[Feature Auditing]]
- [[Fairness Auditing]]
- [[Causal Analysis]]
- [[Feature Governance]]

## Measurement / Evaluation

Proxy relationships may be investigated using:

- correlation analysis
- mutual information
- subgroup analysis
- feature importance
- causal analysis
- predictive reconstruction of protected attributes

However, correlation alone does not determine whether a variable is ethically unacceptable.

Context and purpose matter.

## Ethical Tensions

- [[Fairness vs Predictive Utility]]
- [[Privacy vs Fairness Auditing]]
- [[Protected Attribute Use vs Fairness]]
- [[Feature Utility vs Indirect Discrimination]]

## Key Sources

-

## Open Questions

- When does a correlated feature become an unacceptable proxy?
- Should protected attributes sometimes be collected to detect proxy discrimination?
- Can proxy use be legitimate when it substantially improves safety or accuracy?