---
type: concept
status:
  - developing
domains:
  - bias-fairness
  - ethical-tradeoffs
aliases:
  - Fairness Impossibility Theorems
  - Incompatible Fairness Criteria
created:
  "{ date:YYYY-MM-DD }":
updated:
visibility: private
publish: false
---
## Definition

Fairness impossibility results show that multiple plausible statistical definitions of algorithmic fairness generally cannot be satisfied simultaneously, except under restrictive or degenerate conditions.

The conflict becomes particularly important when:

- outcome prevalence differs across groups
- predictions are imperfect
- fairness criteria condition on different statistical quantities

These results imply that fairness cannot usually be reduced to maximizing a single universal set of statistical constraints.

## Core Idea

Different fairness criteria formalize different normative conceptions of fairness.

For example:

- [[Demographic Parity]] focuses on equality of positive decision rates.
- [[Equal Opportunity]] focuses on equality of true-positive rates.
- [[Equalized Odds]] focuses on equality of error behaviour conditional on the true outcome.
- [[Predictive Parity]] focuses on equality of predictive value conditional on a positive prediction.
- [[Calibration]] focuses on consistency in the empirical meaning of predicted scores.

Because these criteria impose different conditional relationships between predictions, outcomes, and group membership, they may become mathematically incompatible.

## Statistical Perspective

Let:

- `A` = protected group
- `Y` = observed outcome
- `Ŷ` = predicted binary outcome
- `S` = predicted risk score

Several common fairness criteria can be expressed as conditional independence relations.

### Demographic Parity

\[
\hat{Y} \perp A
\]

The prediction should be independent of group membership.

### Equalized Odds

\[
\hat{Y} \perp A \mid Y
\]

Conditional on the true outcome, prediction behaviour should not depend on group membership.

### Predictive Parity / Sufficiency

\[
Y \perp A \mid \hat{Y}
\]

Conditional on the prediction, the observed outcome should not depend on group membership.

### Groupwise Calibration

For a risk score `S`:

\[
P(Y=1 \mid S=s, A=a) = s
\]

for each relevant group `a`.

These criteria condition on different variables and therefore encode fundamentally different fairness objectives.

## Key Impossibility Result

Suppose two groups have different outcome prevalences:

\[
P(Y=1 \mid A=a)
\neq
P(Y=1 \mid A=b)
\]

and the classifier is imperfect.

Then, in general, a classifier cannot simultaneously satisfy both:

- [[Equalized Odds]]
- [[Predictive Parity]]

except in special or degenerate cases.

This is closely related to foundational results by Kleinberg, Mullainathan & Raghavan and Chouldechova.

## Why Base Rates Matter

Let:

\[
\pi_a = P(Y=1 \mid A=a)
\]

denote the base rate for group `a`.

Positive Predictive Value can be written as:

\[
PPV_a =
\frac{TPR_a \pi_a}
{TPR_a \pi_a + FPR_a(1-\pi_a)}
\]

If [[Equalized Odds]] holds, then:

\[
TPR_a = TPR_b
\]

and:

\[
FPR_a = FPR_b
\]

But if:

\[
\pi_a \neq \pi_b
\]

then the PPV values will generally differ:

\[
PPV_a \neq PPV_b
\]

Therefore [[Predictive Parity]] fails.

## Numerical Example

Assume two groups have different base rates:

### Group A

\[
P(Y=1)=0.20
\]

### Group B

\[
P(Y=1)=0.50
\]

Suppose the classifier has identical error behaviour for both groups:

\[
TPR = 0.80
\]

\[
FPR = 0.10
\]

Therefore, [[Equalized Odds]] is satisfied.

For Group A:

\[
PPV_A =
\frac{0.80 \times 0.20}
{0.80 \times 0.20 + 0.10 \times 0.80}
\]

\[
PPV_A \approx 0.67
\]

For Group B:

\[
PPV_B =
\frac{0.80 \times 0.50}
{0.80 \times 0.50 + 0.10 \times 0.50}
\]

\[
PPV_B \approx 0.89
\]

Thus:

\[
PPV_A \neq PPV_B
\]

The classifier satisfies Equalized Odds but violates Predictive Parity.

## Interpretation

Nothing necessarily changed in the classifier's TPR or FPR across groups.

The difference in predictive value arises because the underlying prevalence differs.

This demonstrates why an observed fairness-metric disparity cannot always be interpreted as evidence of different algorithmic treatment.

## Calibration Conflict

Related impossibility results arise between [[Calibration]] and error-rate parity.

A calibrated risk score may assign probabilities that accurately reflect outcome risk within each group.

However, when outcome prevalence differs across groups, imposing equal error rates may require altering scores or thresholds in ways that disrupt calibration.

Therefore:

> Calibration and error-rate parity generally cannot all be simultaneously maintained under unequal base rates and imperfect prediction.

## Special Cases

The incompatibility may disappear under restrictive conditions.

### Equal Base Rates

If:

\[
P(Y=1 \mid A=a)
=
P(Y=1 \mid A=b)
\]

some fairness criteria may become jointly achievable.

### Perfect Prediction

If the classifier predicts outcomes perfectly:

\[
FPR = 0
\]

and:

\[
FNR = 0
\]

many fairness conflicts disappear.

### Degenerate Prediction

Certain trivial classifiers can also technically satisfy multiple constraints, but may provide little or no useful predictive information.

Therefore, impossibility results primarily concern realistic, imperfect predictive systems.

## What the Impossibility Result Does NOT Mean

The theorem does **not** imply:

- fairness is impossible
- fairness analysis is meaningless
- organizations may arbitrarily choose any fairness metric
- every observed disparity is acceptable
- mathematical fairness criteria should be abandoned

Instead, it demonstrates that:

> Fairness requires explicit normative prioritization.

## Ethical Significance

When fairness criteria conflict, selecting a metric becomes an ethical and governance decision rather than a purely technical optimization problem.

The choice depends on questions such as:

- Which error creates the greatest harm?
- Which population bears that harm?
- Is equality of opportunity more important than equality of predictive reliability?
- Should historical base-rate differences be treated as legitimate?
- Are observed labels themselves ethically valid?
- Which stakeholders should participate in defining fairness?

## Example: Hiring

Suppose historical qualification rates differ between two groups.

A hiring model could be optimized for:

### Equal Opportunity

Qualified applicants from both groups have equal probability of being selected.

or:

### Predictive Parity

Among selected candidates, the proportion who subsequently perform well is equal across groups.

If underlying outcome prevalence differs, satisfying both criteria may not be possible simultaneously.

The organization therefore needs to justify which objective is ethically more important for the specific decision.

## Example: Healthcare

Consider a diagnostic model.

One fairness objective could prioritize:

[[Equal Opportunity]]

so patients with a disease are equally likely to be detected across groups.

Another could prioritize:

[[Predictive Parity]]

so a positive diagnosis has equal reliability across groups.

If disease prevalence differs, these criteria may conflict.

The ethical decision depends on the relative harm of:

- missed diagnoses
- unnecessary treatment
- unequal access
- misleading risk communication

## Connection to Multi-Objective Ethics

Fairness impossibility results support viewing Responsible AI as a [[Multi-Objective Ethics]] problem.

AI systems may simultaneously need to balance:

- [[0120 Fairness]]
- [[Accuracy]]
- [[Calibration]]
- [[Privacy]]
- [[Transparency]]
- [[Safety]]
- [[Human Autonomy]]

There may be no single solution that simultaneously maximizes every desirable property.

## Governance Implication

A responsible fairness process should therefore document:

1. which fairness criteria were considered
2. which stakeholders are affected
3. which harms are associated with FP and FN errors
4. whether base rates differ
5. whether base rates themselves may reflect injustice
6. which fairness criterion was selected
7. why that criterion was selected
8. which competing criteria are violated
9. what residual risks remain
10. how fairness will be monitored after deployment

## Common Misinterpretation

A problematic argument is:

> "Fairness metrics conflict, therefore any fairness choice is defensible."

This does not follow.

Impossibility results establish mathematical incompatibility, not ethical equivalence between available choices.

A fairness criterion still requires contextual and normative justification.

## Another Important Caveat

Observed base rates are not necessarily morally neutral.

Differences in:

\[
P(Y=1 \mid A=a)
\]

may themselves result from:

- [[Historical Bias]]
- [[Structural Inequality]]
- [[Measurement Bias]]
- [[Label Bias]]
- unequal access to opportunities
- institutional discrimination

Therefore:

> Statistical prevalence should not automatically be treated as normative ground truth.

## Related Concepts

- [[0140 Fairness Metric Conflicts]]
- [[Base Rate]]
- [[Equalized Odds]]
- [[Predictive Parity]]
- [[Calibration]]
- [[Equal Opportunity]]
- [[Demographic Parity]]
- [[Fairness vs Performance]]
- [[Multi-Objective Ethics]]
- [[Ethical Trade-offs]]
- [[Stakeholder Analysis]]

## Key Insight

> The question is usually not "Which fairness metric is mathematically correct?"

> The more appropriate question is "Which conception of fairness is ethically justified for this decision context, and what harms arise from choosing it over competing alternatives?"

## Open Questions

- Who has legitimate authority to select a fairness criterion?
- How should affected individuals participate in metric selection?
- Should unequal historical base rates ever be treated as ethically neutral?
- How should organizations document unavoidable fairness trade-offs?
- When metrics conflict, should priority be given to equality of errors, outcomes, opportunities, or predictive meaning?
- How should approximate rather than exact fairness be evaluated?


## Key Sources - [[Kleinberg et al. 2017 - Inherent Trade-Offs in the Fair Determination of Risk Scores]] - [[Chouldechova 2017 - Fair Prediction with Disparate Impact]] - [[Pleiss et al. 2017 - On Fairness and Calibration]]