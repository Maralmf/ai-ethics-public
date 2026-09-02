---
type: moc
status: mature
domains: []
created:
updated: 2026-09-01
---

## Purpose

This learning path moves from identifying ethical concerns to analyzing how they arise, how they can be evaluated, and how organizations can respond through measurement, auditing, mitigation, documentation, oversight, assessment, and governance.

It assumes familiarity with the foundational concepts introduced in:

→ [003 Learning Path - Beginner](<003 Learning Path - Beginner>)

The focus is not yet on advanced causal fairness, formal impossibility results, advanced explainability methods, or specialized assurance techniques.

Instead, the goal is to develop **practical analytical competence**:

> moving from identifying an ethical concern to examining its mechanism, evidence, operationalization, controls, and governance implications.

The sequence is pedagogical rather than taxonomic.

---

## Learning Outcomes

By the end of this learning path, you should be able to:

- identify major mechanisms through which bias can enter an AI-enabled decision system
- distinguish historical, representation, selection, sampling, measurement, label, proxy, model, evaluation, deployment, and feedback-related sources of bias
- distinguish a real-world construct from the variable used to measure or predict it
- evaluate whether a target or label is a defensible representation of the construct of interest
- interpret basic classification errors and subgroup performance differences
- explain the logic behind major group fairness criteria
- distinguish group, individual, and intersectional fairness
- explain why fairness metric selection requires normative justification
- recognize when different fairness criteria reflect competing objectives
- structure a basic fairness audit
- distinguish fairness measurement from fairness mitigation
- distinguish technical mitigation from organizational and governance controls
- distinguish explanation methods from documentation artifacts
- evaluate whether human oversight is meaningful in practice
- identify important data-governance requirements
- explain the roles of contestability, redress, auditability, and traceability
- understand the purpose and limitations of AI impact assessment
- distinguish risk assessment from risk acceptance
- explain how evidence should inform governance decisions

---

# Stage 1 — How Bias Enters an AI System

1. [Historical Bias](<0101 Historical Bias>)
2. [Representation Bias](<0102 Representation Bias>)
3. [Selection Bias](<0103 Selection Bias>)
4. [Sampling Bias](<0104 Sampling Bias>)
5. [Measurement Bias](<0105 Measurement Bias>)
6. [Label Bias](<0106 Label Bias>)
7. [Proxy Bias](<0107 Proxy Bias>)
8. [Aggregation Bias](<0108 Aggregation Bias>)
9. [Algorithmic Bias](<0109 Algorithmic Bias>)
10. [Evaluation Bias](<0110 Evaluation Bias>)
11. [Deployment Bias](<0111 Deployment Bias>)
12. [Feedback Loop Bias](<0112 Feedback Loop Bias>)

### Key Question

> At what points in the socio-technical lifecycle can systematic distortion or disadvantage arise?

### Core Insight

Bias should not automatically be attributed to the algorithm.

Potential mechanisms exist across the lifecycle:

**Historical & Institutional Context**

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

**Model Assumptions & Design**

↓

**Evaluation**

↓

**Deployment**

↓

**Feedback**

These categories can interact and overlap.

They should not be treated as mutually exclusive stages or as a deterministic causal chain.

### Important Distinctions

**Historical Bias**

asks whether the underlying social or institutional reality already reflects inequality or disadvantage.

**Representation Bias**

asks whether important populations or contexts are adequately represented.

**Selection Bias**

asks what mechanisms determine which observations become available.

**Sampling Bias**

asks whether the selected sample systematically differs from the target population.

**Measurement Bias**

asks whether the underlying construct is observed appropriately.

**Label Bias**

asks whether the target or recorded outcome is a defensible representation of what the system is intended to predict.

**Proxy Bias**

asks whether apparently neutral features operate as substitutes for ethically salient characteristics.

**Aggregation Bias**

asks whether heterogeneous populations are being modeled under inappropriate common assumptions.

**Algorithmic Bias**

asks whether modeling, optimization, threshold, or decision-rule choices create or amplify systematic disadvantage.

**Evaluation Bias**

asks whether evaluation data, benchmarks, metrics, or procedures adequately represent the intended deployment conditions and relevant harms.

**Deployment Bias**

asks whether the system is being used in a context or manner inconsistent with its design assumptions.

**Feedback Loop Bias**

asks whether system decisions alter the environment in ways that reinforce future patterns.

### Core Principle

> **Different bias mechanisms require different interventions.**

---

# Stage 2 — Ground Truth, Measurement & Construct Validity

13. [Ground Truth](<Ground Truth>)
14. [Construct Validity](<Construct Validity>)
15. [Measurement Bias](<0105 Measurement Bias>)
16. [Label Bias](<0106 Label Bias>)

### Key Question

> Does the variable being measured or predicted validly represent the construct we actually care about?

### Core Insight

Machine-learning systems operate on observable variables and recorded labels.

Ethical and scientific questions often concern broader constructs such as:

- merit
- risk
- ability
- need
- creditworthiness
- productivity
- health status

A recorded variable is not automatically equivalent to the construct it is intended to represent.

For example:

**historical promotion decision**

does not necessarily equal:

**employee merit**

Likewise:

**past arrest**

does not necessarily equal:

**criminal behavior**

and:

**healthcare expenditure**

does not necessarily equal:

**healthcare need**

Therefore:

> **High predictive performance with respect to a recorded target does not establish that the target validly represents the construct of interest.**

A model can accurately reproduce an invalid, incomplete, biased, or ethically problematic target.

### Reasoning Chain

**Construct of Interest**

↓

**Operational Definition**

↓

**Measurement**

↓

**Recorded Variable / Label**

↓

**Model Target**

↓

**Prediction**

Each transition can introduce assumptions that require justification.

---

# Stage 3 — Understanding Classification Errors

17. [Confusion Matrix](<Confusion Matrix>)
18. [Base Rate](<Base Rate>)
19. [True Positive Rate](<True Positive Rate>)
20. [False Positive Rate](<False Positive Rate>)
21. [False Negative Rate](<False Negative Rate>)
22. [Accuracy](Accuracy)

### Key Question

> Who experiences which types of error, and what are the consequences?

### Core Insight

Aggregate accuracy can conceal unequal patterns of error.

For example:

> **Equal accuracy does not imply equal false-positive rates or equal false-negative rates.**

Different errors may also have very different consequences.

A false positive in:

- spam filtering
- medical diagnosis
- fraud detection
- policing
- employment screening

does not carry the same ethical significance.

The relevant question is therefore not only:

> How frequently does the model make an error?

but also:

> **Which error occurs, to whom, under what conditions, and with what consequences?**

### Important

Performance metrics are descriptive evidence.

They do not determine by themselves whether a disparity is ethically acceptable.

---

# Stage 4 — From Fairness Concepts to Fairness Criteria

23. [Group Fairness](<0121 Group Fairness>)
24. [Individual Fairness](<0122 Individual Fairness>)
25. [Intersectional Fairness](<0123 Intersectional Fairness>)

Related:

- [Procedural Fairness](<0124 Procedural Fairness>)
- [Substantive Fairness](<0125 Substantive Fairness>)

### Key Question

> Fair according to what conception of fairness, and fair to whom?

### Core Insight

Fairness is fundamentally a **normative concept**.

Statistical fairness criteria operationalize particular fairness concerns.

They are not complete definitions of ethical fairness.

### Group Fairness

asks whether specified statistical properties differ across socially or ethically relevant groups.

### Individual Fairness

asks whether individuals considered relevantly similar are treated similarly.

Its central challenge is:

> Similar according to what ethically justified notion of similarity?

### Intersectional Fairness

asks whether analyses that examine categories separately may overlook disadvantage occurring at their intersections.

For example:

```text
gender analysis
+
race analysis
