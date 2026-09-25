---
type: moc
status: mature
domains:
  - bias-fairness
created: 2026-09-01
updated: 2026-09-25
---

# Bias & Fairness

## Scope

This MOC organizes concepts related to bias, discrimination, fairness, statistical disparities, fairness criteria, auditing, mitigation, and lifecycle monitoring in AI systems.

It distinguishes among:

- sources of bias
- observed disparities
- normative conceptions of fairness
- statistical fairness criteria
- discriminatory outcomes or practices
- auditing methods
- mitigation strategies
- residual fairness risks

The central questions are:

> **Where can systematic disadvantage enter an AI-enabled decision system?**

> **What conception of fairness is relevant in this context?**

> **How should that conception be operationalized, evaluated, and justified?**

---

## Why This Domain Matters

AI systems can reproduce, amplify, transform, or sometimes reduce existing inequalities.

A system may exhibit high aggregate performance while still producing:

- unequal error rates
- unequal access to opportunities
- disproportionate burdens
- exclusion of particular populations
- systematic disadvantage
- discriminatory outcomes
- reinforcing feedback loops

However:

> **A statistical disparity is not automatically evidence of unfairness, discrimination, or injustice.**

Similarly:

> **The absence of a particular statistical disparity does not establish that a system is ethically fair.**

Fairness evaluation therefore requires both:

**empirical analysis**

and

**normative reasoning**

---

# Conceptual Orientation

A useful reasoning structure is:

**Social & Institutional Context**

↓

**Data-Generating Process**

↓

**Sampling & Representation**

↓

**Measurement & Labels**

↓

**Features & Proxies**

↓

**Model Development**

↓

**Decision Rule**

↓

**Deployment Context**

↓

**Observed Outcomes**

↓

**Disparity Analysis**

↓

**Fairness Criterion**

↓

**Ethical Interpretation**

↓

**Mitigation / Governance**

↓

**Monitoring**

Bias may enter at multiple points in this chain.

Fairness is therefore not a property of the algorithm alone.

---

# Bias

- Bias

The term **bias** is used in several different senses across statistics, machine learning, social science, and ethics.

This distinction matters.

### Statistical Bias

A systematic difference between an estimator's expected value and the quantity it is intended to estimate.

### Data or Measurement Bias

Systematic distortion introduced through sampling, measurement, labeling, representation, or data-generation processes.

### Social or Institutional Bias

Patterns of disadvantage associated with existing social structures, institutional practices, stereotypes, or historical inequalities.

### Algorithmic Bias

Systematic patterns in algorithmic outputs or AI-enabled decisions that may create, reproduce, or amplify disadvantage.

Therefore:

> **Bias should not be treated as a single unified technical phenomenon.**

---

# Sources of Bias

## Historical Bias

- Historical Bias

Occurs when the social or institutional reality reflected in the data already contains inequities or discriminatory patterns.

### Core Insight

Perfectly sampled historical data can still encode historical injustice.

---

## Representation Bias

- Representation Bias

Occurs when relevant populations, environments, behaviors, or conditions are inadequately represented in the available data.

---

## Sampling Bias

- Sampling Bias

Occurs when the mechanism used to select observations systematically produces a sample that differs from the target population in relevant ways.

### Relationship

Sampling bias may contribute to representation bias, but the concepts are not identical.

---

## Selection Bias

- Selection Bias

Occurs when inclusion in the observed dataset depends systematically on variables related to the phenomenon being analyzed.

Selection bias is a broader statistical concept and may arise before, during, or after sampling.

---

## Measurement Bias

- Measurement Bias

Occurs when observed variables measure the underlying construct differently or inaccurately across populations, contexts, or conditions.

Related:

- Construct Validity
- Measurement Error

---

## Label Bias

- Label Bias

Occurs when target labels encode subjective, institutional, historically contingent, or systematically distorted judgments rather than a defensible representation of the underlying construct.

Example:

**historical hiring decision**

does not necessarily equal:

**true job suitability**

Related:

- Ground Truth
- Construct Validity

---

## Proxy Bias

- Proxy Bias

Occurs when apparently neutral variables act as substitutes for protected or ethically salient characteristics.

Examples may include variables correlated with:

- socioeconomic position
- ethnicity
- disability
- geography
- gender

Removing the protected characteristic itself therefore does not necessarily eliminate group-related information.

Related:

- Fairness Through Unawareness

---

## Aggregation Bias

- Aggregation Bias

Occurs when a single model or decision rule is applied across heterogeneous populations whose relationships between features, outcomes, or relevant constructs differ.

---

## Algorithmic Bias

- Algorithmic Bias

May emerge through:

- objective-function design
- model specification
- optimization choices
- threshold selection
- feature engineering
- regularization
- class imbalance
- interaction with biased data

Algorithmic bias should not automatically be interpreted as the sole cause of an observed disparity.

---

## Evaluation Bias

- Evaluation Bias

Occurs when evaluation data, metrics, benchmarks, or testing procedures do not adequately represent the deployment population or ethically relevant performance dimensions.

---

## Deployment Bias

- Deployment Bias

Occurs when a system is used in a context, population, workflow, or purpose that differs materially from the conditions assumed during development or evaluation.

---

## Feedback Loop Bias

- Feedback Loop Bias

Occurs when previous model outputs influence future data in ways that reinforce or amplify existing patterns.

A simplified mechanism is:

**Prediction**

↓

**Decision**

↓

**Behavior / Institutional Response**

↓

**New Data**

↓

**Retraining**

↓

**Stronger Existing Pattern**

Related:

- Feedback Loop
- Fairness Drift

---

# Bias Is Not the Same as Fairness

- Bias vs Fairness

Bias and fairness address different questions.

### Bias

asks:

> Where does systematic distortion or disadvantage come from?

### Fairness

asks:

> What treatment, procedure, outcome, or distribution should count as fair?

Therefore:

> A system can contain bias without every consequence being ethically unfair, and an unfair system may exist even when no single identifiable technical bias is present.

Fairness is fundamentally normative.

---

# Fairness

- Fairness

Fairness concerns whether treatment, procedures, outcomes, opportunities, or distributions of error satisfy a defensible conception of fair treatment.

There is no single universally applicable mathematical definition of fairness.

Different fairness criteria formalize different normative concerns.

Therefore:

> **Fairness metrics are operationalizations of particular fairness concepts, not complete definitions of ethical fairness.**

---

# Group Fairness

- Group Fairness

Group fairness evaluates whether specified outcomes or performance characteristics satisfy some form of parity across groups.

Examples include parity in:

- positive decision rates
- true-positive rates
- false-positive rates
- predictive values
- score calibration

Group fairness is particularly useful for identifying systematic patterns affecting populations.

However:

> Group-level parity does not guarantee fair treatment of every individual.

---

# Individual Fairness

- Individual Fairness

A common formulation is:

> Similar individuals should be treated similarly.

The central challenge is determining:

> Similar according to what ethically and task-relevant notion of similarity?

Individual fairness therefore depends critically on:

- distance definitions
- relevant characteristics
- normative judgments about similarity

---

---

# Intersectional Fairness

- Intersectional Fairness

Fairness evaluated separately across single attributes may conceal harms affecting intersections of characteristics.

For example:

```text
gender analysis
+
age analysis
```

does not necessarily reveal patterns affecting:

```text
gender × age intersections
```

Intersectional analysis can reveal heterogeneity hidden by broader group averages.

However, greater granularity may also create:

- smaller subgroup sizes
- greater statistical uncertainty
- unstable estimates
- multiple-comparison problems
- privacy and re-identification risks

Therefore:

> **Greater subgroup granularity can reveal important disparities, but it does not automatically produce more reliable or ethically sufficient evidence.**

Related:

- Small-Group Uncertainty
- Subgroup Analysis
- Intersectional Analysis

---

# Procedural and Substantive Fairness

## Procedural Fairness

- Procedural Fairness

Procedural fairness concerns whether the decision-making process itself is justifiable.

Relevant questions may include:

- Were decision rules applied consistently?
- Were affected stakeholders treated respectfully?
- Can decisions be understood and challenged?
- Is meaningful review available?
- Are decision-makers appropriately impartial?
- Are relevant procedures transparent enough for scrutiny?

## Substantive Fairness

- Substantive Fairness

Substantive fairness concerns whether the outcomes, burdens, opportunities, or social effects of a decision are fair in context.

A process may appear procedurally consistent while still reproducing serious disadvantage.

Conversely, a favorable aggregate outcome does not necessarily establish that the process was legitimate.

### Core Principle

> **Procedural fairness and substantive fairness are related but non-interchangeable dimensions of ethical evaluation.**

---

# Fairness and Non-Discrimination

- Non-Discrimination
- Fairness vs Non-Discrimination

Fairness and non-discrimination overlap, but they should not automatically be treated as synonyms.

Statistical fairness criteria may help detect or characterize disparities.

Non-discrimination may involve:

- ethical requirements
- rights-based constraints
- jurisdiction-specific legal definitions
- protected characteristics
- justification tests
- remedies

Therefore:

> **Satisfying a statistical fairness criterion does not by itself establish compliance with non-discrimination requirements or ethical acceptability.**

Likewise:

> **Failure to satisfy a particular fairness metric does not by itself establish unlawful discrimination.**

Legal conclusions require analysis of the applicable legal framework.

Related:

→ 007 MOC - Human Rights Justice & Inclusion

---

# Disparity, Bias, Discrimination & Injustice

These concepts should remain distinct.

### Disparity

An observed difference between groups, individuals, or outcomes.

### Bias

A mechanism or systematic distortion that may contribute to a disparity or disadvantage.

### Discrimination

Unjustified disadvantage connected to protected or otherwise ethically salient characteristics, with legal meaning depending on jurisdiction.

### Injustice

A broader normative judgment concerning unjust treatment, distribution, institutions, or social relations.

A useful caution is:

> **Disparity ≠ Bias ≠ Discrimination ≠ Injustice**

An observed disparity may justify investigation without establishing its cause or ethical status.

Conversely, an ethically problematic system may exist even when one selected disparity measure is small or absent.

Related:

- Disparity vs Bias
- Disparity vs Discrimination
- Fairness vs Justice

---

# Statistical Fairness Criteria

Statistical fairness criteria operationalize particular concerns through measurable relationships.

They should be interpreted in relation to:

- the decision context
- target validity
- affected rights
- error consequences
- group definitions
- uncertainty
- stakeholder interests
- available alternatives

They are analytical tools, not complete ethical theories.

---

## Demographic Parity

- Demographic Parity

A common formulation requires parity in the rate of a selected outcome across groups:

\[
P(\hat{Y}=1 \mid A=a)
\]

being equal across relevant values of \(A\).

### Ethical Question

> Should different groups receive positive decisions at similar rates in this context?

### Limitations

Demographic parity does not by itself establish that:

- the underlying target is valid
- individuals are similarly situated
- error burdens are fairly distributed
- historical disadvantage has been addressed
- the decision process is legitimate

---

## Equal Opportunity

- Equal Opportunity

A common formulation requires parity in the true-positive rate across groups:

\[
P(\hat{Y}=1 \mid Y=1,A=a)
\]

being equal across relevant groups.

### Ethical Question

> Among those labeled positive by the reference outcome, should groups have comparable opportunity to receive a positive prediction?

### Important

The ethical relevance of Equal Opportunity depends partly on whether \(Y\) is itself a defensible reference outcome.

If the label reflects historical injustice or invalid measurement, parity relative to that label may not resolve the underlying problem.

---

## Equalized Odds

- Equalized Odds

A common formulation is:

\[
\hat{Y} \perp A \mid Y
\]

For binary classification, this implies parity in relevant error rates such as:

- True Positive Rate
- False Positive Rate

### Ethical Question

> Should error behavior be similar across groups conditional on the reference outcome?

Equalized Odds can be useful where both false-positive and false-negative disparities are ethically relevant.

---

## Predictive Parity

- Predictive Parity

A common formulation focuses on parity in Positive Predictive Value:

\[
P(Y=1 \mid \hat{Y}=1,A=a)
\]

being equal across groups.

### Important

> **Ordinary Predictive Parity should not automatically be treated as equivalent to full conditional independence of \(Y\) and \(A\) given \(\hat{Y}\).**

The latter is a stronger condition.

### Ethical Question

> Should a positive prediction carry comparable evidential meaning across groups?

---

## Calibration

- Calibration

For a probabilistic score \(S\), groupwise calibration may be expressed as:

\[
P(Y=1 \mid S=s,A=a)=s
\]

for relevant scores and groups.

Conceptually:

> among people assigned the same predicted risk, observed outcome frequencies should correspond appropriately to that risk estimate.

Calibration can support interpretation of risk scores.

However:

> **Calibration does not by itself establish fairness, causal validity, or ethical legitimacy.**

---

# Fairness Metric Selection

- Fairness Metric Selection

Choosing a fairness criterion is not merely a technical parameter-selection problem.

The choice should be justified by questions such as:

- What decision is being made?
- Which errors matter most?
- Who bears those errors?
- What rights or opportunities are affected?
- Is the target variable valid?
- Which groups require analysis?
- What historical disadvantage is relevant?
- What alternatives exist?
- What legal or institutional requirements apply?

Therefore:

> **A fairness metric should be selected because it operationalizes a justified fairness concern—not because it is convenient or easy to optimize.**

Related:

→ 017 MOC - Ethical Trade-offs & Decision Reasoning

---

# Fairness Metric Conflicts

- Fairness Metric Conflicts

Different fairness criteria may produce different evaluations of the same system because they condition on different quantities and represent different operational concerns.

Examples include potential tension among:

- selection-rate parity
- error-rate parity
- predictive-value parity
- calibration

A metric conflict does not automatically imply an ethical trade-off.

First ask:

- Do the criteria represent genuinely competing normative objectives?
- Is the conflict caused by current design choices?
- Could better data or measurement reduce the conflict?
- Is the target itself defensible?
- Could a different decision process avoid the conflict?

### Core Principle

> **Statistical incompatibility and ethical conflict are related questions, not identical ones.**

---

# Fairness Impossibility Results

- Fairness Impossibility Results

Under particular statistical assumptions—commonly involving unequal observed base rates and imperfect prediction—certain combinations of fairness criteria cannot generally all be satisfied simultaneously except under special conditions.

The exact claim depends on:

- the fairness definitions involved
- whether predictions are binary decisions or scores
- assumptions about calibration
- error rates
- prevalence
- prediction quality

Therefore impossibility results should not be summarized as:

> "fairness metrics always conflict."

They do not imply that:

- fairness itself is impossible
- every metric is equally defensible
- disparities may be ignored
- mathematics determines the ethical answer

Instead:

> **Formal incompatibility exposes the need for explicit normative justification.**

---

# Base Rates

- Base Rate

Observed outcome prevalence may differ across groups:

\[
P(Y=1 \mid A=a)
\]

Base-rate differences can affect relationships among statistical fairness criteria.

However:

> **Observed base-rate differences should not automatically be treated as natural, legitimate, or ethically neutral.**

They may reflect:

- historical conditions
- unequal opportunity
- institutional practices
- measurement choices
- structural inequality
- differential exposure
- selection processes

Therefore base rates are empirical facts to interpret, not normative conclusions.

---

# Construct Validity & Ground Truth

- Construct Validity
- Ground Truth

Fairness analysis can be misleading when the target variable poorly represents the construct of interest.

Examples:

```text
historical hiring decision
≠
true job suitability
```

```text
past arrest
≠
criminal behavior
```

```text
healthcare expenditure
≠
healthcare need
```

A model can predict a recorded target accurately while reproducing an invalid, incomplete, or biased construct.

Therefore:

> **High predictive performance relative to a label does not establish that the label is ethically or scientifically defensible.**

Fairness evaluation should examine:

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

Each transition introduces assumptions.

---

# Fairness Auditing

- Fairness Audit

A fairness audit should evaluate more than a small set of parity metrics.

A robust audit may examine:

1. **Purpose & Decision Context**
2. **Affected Stakeholders**
3. **Data-Generating Process**
4. **Selection & Representation**
5. **Construct & Measurement Validity**
6. **Labels & Targets**
7. **Subgroup Performance**
8. **Relevant Fairness Criteria**
9. **Statistical Uncertainty**
10. **Intersectional Patterns**
11. **Severity & Distribution of Harms**
12. **Potential Root Causes**
13. **Existing Technical Controls**
14. **Organizational & Governance Controls**
15. **Residual Fairness Risk**
16. **Monitoring & Reassessment**

### Important

An observed disparity does not automatically identify:

- the causal mechanism
- the responsible actor
- the ethically relevant explanation
- the appropriate intervention

### Core Principle

> **Fairness auditing should support diagnosis and governance, not merely produce a compliance score.**

---

# Uncertainty in Fairness Evaluation

Fairness estimates are themselves uncertain.

Relevant sources may include:

- small subgroup sizes
- sampling variation
- measurement error
- label uncertainty
- multiple comparisons
- distribution shift
- missing data
- changing populations

A point estimate such as:

> Group A FPR = 12%, Group B FPR = 16%

should not automatically be interpreted as a stable or practically meaningful difference without considering:

- sample size
- uncertainty intervals where appropriate
- effect magnitude
- decision consequences
- temporal stability

### Core Principle

> **Fairness analysis should report uncertainty rather than treating estimated disparities as exact facts.**

---

# Causal Analysis of Fairness

- Causal Fairness
- Causal Inference

Statistical disparity does not identify why the disparity exists.

For example:

\[
FPR_A \neq FPR_B
\]

does not establish whether the difference results from:

- historical conditions
- selection
- measurement
- confounding
- labels
- model behavior
- thresholds
- institutional processes
- deployment practices

Causal analysis may help distinguish mechanisms.

However, causal fairness also contains normative choices about:

- which variables matter
- which pathways are legitimate
- which mediators are acceptable
- which counterfactual comparisons are meaningful

Therefore:

> **Causal identification and ethical justification remain distinct tasks.**

---

# Fairness Mitigation

- Fairness Mitigation

Mitigation should follow diagnosis.

Possible interventions include technical, organizational, and governance measures.

---

## Pre-Processing

- Pre-Processing

Potential interventions may involve:

- resampling
- reweighting
- improving representation
- revising measurements
- correcting labels
- removing or transforming problematic features

These methods should not be assumed to repair unjust historical conditions automatically.

---

## In-Processing

- In-Processing

Potential interventions may modify:

- loss functions
- optimization objectives
- fairness constraints
- model architecture
- regularization

An optimized constraint is only as defensible as the fairness concern it represents.

---

## Post-Processing

- Post-Processing

Potential interventions may modify:

- thresholds
- decision rules
- calibration procedures
- human-review routing

Post-processing may change statistical outcomes without addressing upstream causes.

---

## Organizational & Governance Mitigation

Some fairness problems cannot be solved by modifying the model.

Relevant interventions may include:

- changing the decision process
- revising eligibility criteria
- improving appeal procedures
- adding meaningful human review
- narrowing deployment scope
- changing institutional practices
- introducing independent review
- choosing a non-AI alternative

### Core Principle

> **The appropriate mitigation depends on the mechanism producing the ethically relevant harm.**

---

# Fairness vs Performance

- Fairness vs Performance

Fairness and predictive performance may sometimes appear to conflict.

However:

> **A fairness–performance trade-off should be demonstrated rather than assumed.**

Apparent conflict may depend on:

- the chosen performance metric
- the chosen fairness criterion
- model class
- data quality
- target definition
- threshold choices
- evaluation population
- optimization strategy

Redesign may sometimes improve both.

Even when a genuine conflict remains, the technical trade-off does not determine the ethical decision.

The distribution and severity of consequences still require normative justification.

---

# Fairness vs Justice

- Fairness vs Justice

Fairness is not identical to justice.

A system may satisfy a selected fairness metric while remaining unjust because:

- the system's purpose is illegitimate
- the target encodes structural disadvantage
- affected people cannot contest decisions
- privacy or autonomy is violated
- burdens fall on vulnerable groups
- institutional power is unjustly distributed

Therefore:

> **Statistical fairness can contribute evidence to a justice analysis, but it does not define justice.**

Related:

→ 007 MOC - Human Rights Justice & Inclusion

---

# Statistical Fairness vs Ethical Fairness

- Statistical Fairness vs Ethical Fairness

Statistical fairness concerns measurable relationships among predictions, outcomes, and groups.

Ethical fairness concerns whether treatment or outcomes can be justified in relation to:

- context
- rights
- harms
- history
- institutional roles
- affected stakeholders
- alternatives
- power
- uncertainty

Therefore:

> **Satisfying a statistical criterion is neither necessary in every context nor sufficient in every context for ethical fairness.**

The relevance of a metric depends on the normative concern it is intended to operationalize.

---

# Fairness Across the AI Lifecycle

Fairness should be evaluated across the lifecycle rather than only at model validation.

A useful structure is:

**Problem Formulation**

↓

**Data Generation**

↓

**Selection & Representation**

↓

**Measurement & Labels**

↓

**Model Development**

↓

**Evaluation**

↓

**Decision Policy**

↓

**Deployment**

↓

**Monitoring**

↓

**Feedback & Reassessment**

At each stage, ask:

- What assumption is being made?
- Who may be disadvantaged?
- What evidence supports the decision?
- What control is available?
- What residual fairness risk remains?

---

# Fairness Drift

- Fairness Drift

A system that appears acceptable at deployment may develop different fairness properties over time.

Fairness may change because:

- population composition changes
- base rates change
- data collection changes
- labels change
- user behavior adapts
- model versions change
- thresholds change
- deployment scope expands
- institutions respond to system decisions

Therefore:

> **Initial fairness evidence ≠ Permanent fairness**

Related:

- Data Drift
- Concept Drift
- Post-Deployment Monitoring
- 020 MOC - Lifecycle Monitoring & Incident Management

---

# Feedback Loops

AI-enabled decisions can alter the environment that generates future data.

For example:

**Prediction**

↓

**Decision**

↓

**Resource Allocation / Intervention**

↓

**Behavioral or Institutional Change**

↓

**New Observations**

↓

**Future Training Data**

Feedback loops may:

- reinforce prior patterns
- create self-fulfilling predictions
- change observed base rates
- shift who becomes visible in the data
- amplify institutional disadvantage

Therefore longitudinal analysis may be required.

---

# Relationship to Human Rights & Justice

→ 007 MOC - Human Rights Justice & Inclusion

Bias and fairness analysis provides tools for identifying and evaluating disparities.

Human-rights and justice analysis asks broader questions about:

- dignity
- rights
- equality
- discrimination
- legitimacy
- structural disadvantage

A metric should operationalize a justified normative concern.

The arrow should not be reversed automatically:

> **Metric → observed result does not define what justice requires.**

---

# Relationship to Harm, Risk & Power

→ 008 MOC - Harm Risk & Power

A disparity becomes ethically significant partly through its consequences.

Ask:

- What harm may follow?
- How severe is it?
- Who is exposed?
- Who is vulnerable?
- Is the harm reversible?
- Who has power to contest or avoid it?
- What residual risk remains?

Therefore:

> **Disparity analysis and harm analysis are complementary, not interchangeable.**

---

# Relationship to Accountability

→ 014 MOC - Accountability Contestability & Redress

Fairness governance requires:

- clear responsibility
- auditability
- traceability
- contestability
- review
- correction
- redress

Without these mechanisms, affected people may be unable to challenge unfair or erroneous decisions.

---

# Relationship to Governance

→ 018 MOC - Governance Regulation & Legitimacy

Fairness decisions involve institutional choices about:

- relevant groups
- acceptable metrics
- thresholds
- target definitions
- evidence requirements
- mitigation
- residual risk
- monitoring
- escalation
- deployment restrictions

These choices should be documented and assigned to legitimate decision-makers.

---

# Practical Fairness Evaluation Lens

When evaluating an AI-enabled decision system, ask:

## Purpose

- What decision is being supported or automated?
- Is the use of AI itself justified?
- What alternatives exist?

## Stakeholders

- Who benefits?
- Who bears errors or burdens?
- Who has decision-making power?

## Construct

- What real-world construct matters?
- How is it operationalized?
- Is the target a defensible representation?

## Data

- How were data generated?
- Who is missing or poorly represented?
- What selection, sampling, measurement, or label biases may exist?

## Bias Mechanisms

- Where can systematic distortion or disadvantage arise?

## Groups

- Which groups are ethically relevant?
- Are intersectional groups being obscured?

## Errors

- Which error types matter?
- Who experiences them?
- What consequences follow?

## Fairness Criteria

- What fairness concern is relevant?
- Which criterion operationalizes part of that concern?
- What does the metric fail to capture?

## Uncertainty

- How stable are subgroup estimates?
- Are sample sizes adequate?
- What uncertainty should be reported?

## Causal Mechanism

- What may explain the observed disparity?
- What evidence supports that explanation?

## Mitigation

- Which intervention addresses the actual mechanism?
- Could mitigation shift burdens elsewhere?

## Governance

- Who selects the fairness criterion?
- Who accepts residual fairness risk?
- Can affected people challenge the decision?

## Monitoring

- What should be monitored after deployment?
- What evidence should trigger reassessment or intervention?

---

# Example — AI-Assisted Hiring

Consider an AI system used to recommend applicants for employment.

Suppose overall predictive performance is high, but among applicants labeled as qualified in the evaluation data, one group receives positive recommendations less frequently than another.

A rigorous fairness analysis should not jump directly to a metric.

### Historical Bias

Were previous hiring or promotion practices themselves discriminatory?

### Representation

Were relevant applicant populations adequately represented?

### Selection

Who entered the historical dataset, and what processes determined inclusion?

### Measurement

Do observed variables validly measure job-relevant constructs?

### Labels

Does the label "qualified" represent a defensible measure of job suitability?

### Error Analysis

Which groups experience false positives or false negatives, and what are the consequences?

### Fairness Criterion

If similarly qualified applicants should have comparable opportunity to receive a positive recommendation, is an opportunity-based criterion relevant?

### Intersectionality

Do broader group averages hide disparities affecting smaller intersections?

### Causality

What mechanism plausibly explains the disparity?

### Mitigation

Should the intervention target:

- data
- measurement
- labels
- model design
- thresholds
- human review
- the broader hiring process

### Accountability

Who is responsible for evaluating, approving, monitoring, and correcting the system?

### Redress

Can applicants challenge an incorrect decision?

### Monitoring

Could fairness change after deployment as applicant behavior, recruitment, data, or decision practices evolve?

This example illustrates:

> **A fairness metric is one component of a broader socio-technical fairness analysis.**

---

# Common Failure Modes in Fairness Reasoning

### "A disparity proves bias."

Not necessarily.

A disparity is evidence requiring interpretation and investigation.

---

### "Bias proves discrimination."

Not automatically.

Discrimination is a normative and, in legal contexts, jurisdiction-specific conclusion.

---

### "Removing protected attributes prevents discrimination."

Not necessarily.

Proxy variables, historical structure, and correlated information may preserve group-related effects.

---

### "Equal accuracy means equal fairness."

False.

Different groups may experience different error distributions despite similar aggregate accuracy.

---

### "One fairness metric tells us whether the system is fair."

False.

Metrics operationalize specific concerns.

---

### "If a fairness metric is satisfied, the system is ethically fair."

Not necessarily.

The purpose, target, process, rights, harms, and institutional context still matter.

---

### "Fairness metrics always conflict."

Too broad.

Some formal incompatibilities arise only under particular assumptions and definitions.

---

### "Improving fairness necessarily reduces performance."

Not necessarily.

The existence and magnitude of a trade-off must be demonstrated in the relevant context.

---

### "Fairness can be solved entirely at the model level."

False.

Many fairness problems arise from institutions, data-generating processes, measurement, decision policies, and deployment.

---

### "Initial fairness testing is enough."

False.

Fairness can drift over time.

---

# Evidence & Normative Status

Fairness analysis should distinguish among different kinds of claims.

### Empirical Claim

> Group A has a higher false-positive rate than Group B.

### Statistical Inference

> The observed difference is estimated with a particular level of uncertainty.

### Causal Claim

> A specific mechanism produced or contributed to the disparity.

### Normative Claim

> The disparity is unfair or ethically unacceptable.

### Legal Claim

> The practice constitutes unlawful discrimination under an applicable legal framework.

These conclusions require different evidence and forms of justification.

Therefore:

> **Observed disparity does not automatically establish causal bias, ethical unfairness, or legal discrimination.**

Likewise:

> **Absence of one selected disparity does not establish overall ethical fairness.**

---

# Ethical Reasoning Chain

A useful reasoning sequence is:

**Purpose & Decision Context**

↓

**Stakeholders & Power**

↓

**Construct & Target Validity**

↓

**Data-Generating Process**

↓

**Bias Mechanisms**

↓

**Observed Outcomes**

↓

**Disparity & Error Analysis**

↓

**Uncertainty**

↓

**Causal Investigation**

↓

**Normative Fairness Concern**

↓

**Operational Fairness Criterion**

↓

**Metric / Evaluation Method**

↓

**Ethical Interpretation**

↓

**Mitigation & Controls**

↓

**Residual Fairness Risk**

↓

**Governance Decision**

↓

**Monitoring & Reassessment**

This sequence is iterative rather than strictly linear.

New evidence may require earlier assumptions, metrics, or interventions to be reconsidered.

---

# Related MOCs

### Foundations
→ 006 MOC - Foundations & Ethical Theory

### Human Rights & Justice
→ 007 MOC - Human Rights Justice & Inclusion

### Harm, Risk & Power
→ 008 MOC - Harm Risk & Power

### Privacy & Data Governance
→ 010 MOC - Privacy & Data Governance

### Transparency & Explainability
→ 011 MOC - Transparency Interpretability & Explainability

### Human Agency
→ 012 MOC - Human Agency Autonomy & Oversight

### Accountability
→ 014 MOC - Accountability Contestability & Redress

### Ethical Reasoning
→ 017 MOC - Ethical Trade-offs & Decision Reasoning

### Governance
→ 018 MOC - Governance Regulation & Legitimacy

### Responsible AI Engineering
→ 019 MOC - Responsible AI Engineering & Assurance

### Lifecycle
→ 020 MOC - Lifecycle Monitoring & Incident Management

---

# Evidence & Literature Directions

Relevant evidence and literature may include:

## Fairness Foundations

- philosophical and normative theories of fairness and justice
- equality and non-discrimination
- procedural and substantive fairness
- individual and group fairness

## Statistical Fairness

- demographic parity
- equal opportunity
- equalized odds
- predictive parity
- calibration
- base-rate relationships
- formal incompatibility results

## Bias & Measurement

- data-generating processes
- sampling and selection bias
- measurement and construct validity
- label bias
- proxy discrimination
- feedback loops

## Auditing & Mitigation

- fairness auditing
- subgroup and intersectional analysis
- uncertainty reporting
- mitigation techniques
- organizational controls
- lifecycle monitoring

## Causal Fairness

- causal inference
- counterfactual fairness
- pathway-specific reasoning
- normative assumptions in causal models

Specific sources should be maintained as dedicated literature, framework, method, or evidence notes and linked to the relevant concepts.

---

# Open Questions

- Which conception of fairness is relevant in a given AI decision context?
- When should group fairness take priority over individual fairness, or vice versa?
- How should historical disadvantage influence present fairness requirements?
- When is differential treatment ethically justified?
- How should target validity affect fairness evaluation?
- Which group definitions are ethically and statistically appropriate?
- How granular should intersectional analysis become before uncertainty or privacy risk becomes prohibitive?
- How should fairness metrics be selected when multiple legitimate objectives conflict?
- What evidence is required before attributing a disparity to a causal mechanism?
- When should a fairness problem be addressed through organizational redesign rather than model modification?
- How should fairness be monitored under distribution shift?
- What level of residual fairness risk, if any, may legitimately be accepted?
- Who has authority to select fairness criteria and accept residual disparities?
- When should unresolved fairness concerns lead to restricted deployment or non-deployment?
- How should fairness requirements interact with privacy, safety, autonomy, and other ethical constraints?

---

## Continue Exploring

→ 010 MOC - Privacy & Data Governance

→ 011 MOC - Transparency Interpretability & Explainability

→ 012 MOC - Human Agency Autonomy & Oversight

→ 014 MOC - Accountability Contestability & Redress

→ 017 MOC - Ethical Trade-offs & Decision Reasoning

→ 020 MOC - Lifecycle Monitoring & Incident Management
