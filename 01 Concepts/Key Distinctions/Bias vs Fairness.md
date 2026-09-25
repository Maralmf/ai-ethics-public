---
type: concept
status: developing
domains:
  - bias-fairness
aliases:
  - Bias and Fairness
created: 2026-09-01
updated:
visibility: private
publish: false
---
## Core Distinction

[[0100 Bias]] and [[0120 Fairness]] are related but conceptually distinct.

**Bias** primarily concerns the mechanisms through which systematic distortion, disadvantage, or unequal patterns may arise.

**Fairness** concerns the normative evaluation of treatment, procedures, outcomes, opportunities, or error distributions.

A useful working distinction is:

> **Bias asks where systematic distortion or disadvantage may come from.**

> **Fairness asks what should count as fair treatment, and how that judgment should be justified and evaluated.**

Therefore:

> **Bias ≠ Unfairness**

and more generally:

> **Disparity ≠ Bias ≠ Discrimination ≠ Injustice**

These concepts may be related, but none should automatically be inferred from another.

---

# Conceptual Map

A more defensible relationship is:

**Social & Institutional Context**

↓

**Potential Sources of Bias**

↓

**Data / Measurement / Model / Deployment Mechanisms**

↓

**Observed System Behavior**

↓

**Potential Disparities**

↓

**Consequences & Harms**

↓

**Normative Fairness Question**

↓

**Fairness Criterion**

↓

**Metric or Evaluation Method**

↓

**Ethical Interpretation**

↓

**Audit / Mitigation / Governance**

↓

**Monitoring & Reassessment**

This is a reasoning structure, not a deterministic causal chain.

---

# Bias

[[0100 Bias]] is an overloaded term.

It may refer to different phenomena in:

- statistics
- machine learning
- data collection
- social institutions
- measurement
- decision-making

In AI Ethics, bias commonly refers to systematic mechanisms or patterns that may distort representation, measurement, prediction, or decision outcomes.

Bias does **not** automatically imply ethical unfairness.

For example, an observed statistical difference may:

- reflect a legitimate task-relevant distinction
- result from measurement error
- reflect historical inequality
- arise from inappropriate sampling
- result from model or threshold choices
- become ethically problematic only in a particular decision context

Therefore, the ethical significance of bias depends on:

- context
- mechanism
- affected stakeholders
- resulting harms
- rights
- alternatives
- power relationships

---

# Sources of Bias

Bias can enter an AI-enabled decision system at multiple stages.

A useful lifecycle-oriented map is:

**Historical / Social Conditions**

↓

**Representation & Selection**

↓

**Sampling**

↓

**Measurement**

↓

**Labels**

↓

**Features & Proxies**

↓

**Model Design**

↓

**Evaluation**

↓

**Deployment**

↓

**Feedback**

Relevant concepts include:

- [[Historical Bias]]
- [[Representation Bias]]
- [[Selection Bias]]
- [[Sampling Bias]]
- [[Measurement Bias]]
- [[Label Bias]]
- [[Proxy Bias]]
- [[Aggregation Bias]]
- [[Algorithmic Bias]]
- [[Evaluation Bias]]
- [[Deployment Bias]]
- [[Feedback Loop Bias]]

These categories may overlap and interact.

They should not be interpreted as mutually exclusive stages.

---

# Historical Bias

[[0101 Historical Bias]] concerns situations in which the social or institutional reality represented by the data already reflects pre-existing inequality, discrimination, or disadvantage.

### Core Question

> Is the underlying reality represented by the data already ethically problematic?

For example:

**Past unequal social conditions**

↓

[[0104 Sampling Bias]]

↓

may remain present even when

↓

**sampling is statistically representative**

This is important because:

> Representative data can accurately reproduce an unjust reality.

Historical Bias is therefore not solved merely by improving sample representativeness.

---

# Representation Bias

[[0102 Representation Bias]] concerns whether relevant populations, contexts, behaviors, or environments are adequately represented in the available data.

### Core Question

> Are important groups and conditions sufficiently represented in the dataset?

Possible causes include:

- inaccessible data collection
- exclusion from platforms
- geographic imbalance
- language imbalance
- demographic imbalance
- underrepresentation of rare conditions

---

# Selection and Sampling Bias

## Selection Bias

[[Selection Bias]] concerns systematic mechanisms determining which observations become available for analysis.

### Core Question

> Who or what becomes observable, and why?

---

## Sampling Bias

[[0104 Sampling Bias]] concerns whether the process used to select a sample produces systematic differences between the sample and the target population.

### Core Question

> Does the sampling process give some individuals, groups, or conditions systematically different chances of entering the dataset?

A possible relationship is:

**Selection mechanism**

↓

may produce

↓

[[0104 Sampling Bias]]

↓

which may contribute to

↓

[[0102 Representation Bias]]

However:

> Selection Bias, Sampling Bias, and Representation Bias are related but not synonymous.

---

# Measurement Bias

[[0105 Measurement Bias]] concerns systematic distortion in how an underlying construct is operationalized or observed.

A useful reasoning sequence is:

**Real-World Construct**

↓

**Operational Definition**

↓

**Measurement**

↓

**Observed Variable**

### Core Question

> Does the observed variable measure the underlying construct accurately and comparably across relevant groups and contexts?

Examples of constructs include:

- ability
- risk
- productivity
- creditworthiness
- health status

The observable variable is not necessarily identical to the construct it is intended to represent.

---

# Label Bias

[[Label Bias]] concerns systematic problems in the target or outcome treated as ground truth.

A useful distinction is:

**What outcome do we want to understand?**

↓

**What outcome is actually recorded?**

↓

[[0106 Label Bias]]

For example:

**Historical hiring decision**

does not necessarily equal:

**true candidate suitability**

### Core Question

> Is the label a defensible representation of the phenomenon the system is intended to predict?

Labels may encode:

- historical institutional decisions
- human judgment
- subjective assessment
- incomplete observation
- previous discrimination

---

# Proxy Bias

[[0107 Proxy Bias]] concerns variables that appear neutral but function as substitutes for protected or ethically salient characteristics.

A useful reasoning sequence is:

**Construct of Interest**

↓

**Unavailable or Restricted Variable**

↓

**Substitute Variable**

↓

possible correlation with protected characteristic

↓

[[0107 Proxy Bias]]

Examples may include:

- postcode
- purchasing patterns
- educational history
- behavioral traces

Therefore:

> Removing protected attributes does not necessarily remove protected-group information from a model.

Related:

→ [[Fairness Through Unawareness]]

---

# Algorithmic Bias

[[0109 Algorithmic Bias]] concerns systematic patterns in model outputs or AI-enabled decisions that create, reproduce, or amplify disadvantage.

It may arise from biased data, but it may also emerge from choices involving:

- objective functions
- loss functions
- optimization
- feature engineering
- model architecture
- class weighting
- thresholds
- decision rules
- interactions among variables

Therefore, this simplified relation:

**Data Bias**

↓

**Algorithmic Bias**

can sometimes occur, but should not be treated as universally sufficient.

A better representation is:

```text
Historical / Institutional Context
        │
        ├── Data
        ├── Measurement
        ├── Labels
        ├── Features
        ├── Model Design
        ├── Thresholds
        └── Deployment
                ↓
        System Behavior