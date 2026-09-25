## Core Distinction

**Statistical Fairness** asks:

> **Are outcomes, opportunities, or error rates distributed across groups according to a defined mathematical criterion?**

**Ethical Fairness** asks:

> **Is the treatment of individuals and groups actually justified and defensible in this context?**

A useful mental model is:

**Statistical Fairness = Measurable parity**

**Ethical Fairness = Normative justification**

---

## Statistical Fairness

Statistical fairness translates a fairness objective into measurable relationships between groups.

It may examine:

- Selection rates
    
- Approval rates
    
- True Positive Rates
    
- False Positive Rates
    
- False Negative Rates
    
- Calibration
    
- Error distributions
    
- Performance across subgroups
    

Its purpose is to make potential disparities **observable and testable**.

---

## Examples of Statistical Fairness Criteria

### Demographic Parity

Different groups should receive positive outcomes at similar rates.

Example:

> Loan approval rates should be similar across protected groups.

This focuses on the **distribution of outcomes**.

---

### Equal Opportunity

Qualified individuals from different groups should have similar chances of receiving a positive outcome.

Operationally, this often means similar:

> **True Positive Rates**

This focuses on whether people who should receive a positive decision are treated similarly.

---

### Equalized Odds

Both:

- True Positive Rate
    
- False Positive Rate
    

should be similar across groups.

This focuses on the distribution of different types of error.

---

### Calibration

For people receiving the same predicted risk score, actual outcome probabilities should be similar across groups.

Example:

If two groups receive a risk score of 0.8:

> Approximately 80% of each group should actually experience the predicted outcome.

---

## What Statistical Fairness Does Well

Statistical fairness helps answer questions such as:

- Is one group rejected more frequently?
    
- Is one group exposed to more false positives?
    
- Does one group experience more false negatives?
    
- Is predictive quality different across populations?
    
- Has fairness deteriorated after deployment?
    

It turns abstract fairness concerns into:

**Metric → Threshold → Test → Monitoring**

---

# Ethical Fairness

Ethical fairness goes beyond numerical parity.

It asks:

- Which differences in treatment are justified?
    
- Which groups should be compared?
    
- Which outcome matters most?
    
- Which error is more harmful?
    
- What historical context matters?
    
- Are the criteria used by the model legitimate?
    
- Who bears the cost of error?
    
- Does the process respect rights and autonomy?
    
- Can affected individuals challenge the decision?
    

Ethical fairness therefore requires:

**Context + Values + Consequences + Rights + Justification**

---

# Same Numbers, Different Ethical Meaning

Suppose two groups have exactly the same:

- Accuracy
    
- False Positive Rate
    
- False Negative Rate
    

Does this prove the system is ethically fair?

No.

The model may still rely on an ethically questionable feature.

Example:

A hiring system uses:

> Previous unpaid internship experience

The model may produce identical error rates across groups.

But ethical analysis should still ask:

- Is unpaid internship experience a legitimate hiring criterion?
    
- Does it systematically privilege people from wealthier backgrounds?
    
- Is it genuinely relevant to job performance?
    

Therefore:

> **Metric parity does not automatically establish ethical legitimacy.**

---

# Unequal Numbers Can Also Be Ethically Defensible

The reverse is also important.

Statistical equality is not always ethically required.

Example:

A medical system may recommend different treatments to groups with genuinely different clinical needs.

If the differences are based on medically relevant evidence rather than unjustified discrimination, different outcomes may still be ethically defensible.

Therefore:

> **Different treatment ≠ Unfair treatment**

The key question is:

> **Is the difference justified by ethically relevant factors?**

---

# Accuracy Equality Is Not Fairness

Suppose:

|Metric|Group A|Group B|
|---|--:|--:|
|Accuracy|90%|90%|
|False Negative Rate|5%|20%|

Both groups have identical Accuracy.

But Group B experiences four times as many False Negatives.

If the application is medical diagnosis, this disparity may be ethically significant.

Therefore:

> **Aggregate metric equality can hide ethically important differences in error distribution.**

---

# Statistical Fairness Is Metric-Dependent

A model may satisfy one fairness criterion and fail another.

Example:

A model may be well calibrated across groups but have unequal False Positive Rates.

Or it may satisfy Demographic Parity but produce worse calibration.

Therefore:

> **“Is the model statistically fair?” is incomplete.**

The better question is:

> **Fair according to which criterion, and why is that criterion appropriate for this use case?**

---

# Fairness Metric Selection Is an Ethical Choice

Choosing a fairness metric is not purely technical.

Suppose a medical system has two possible fairness objectives:

### Option A

Equal False Positive Rates

### Option B

Equal False Negative Rates

Which should be prioritized?

The answer depends on:

- Clinical consequences
    
- Severity of missed diagnosis
    
- Cost of unnecessary treatment
    
- Vulnerability of affected groups
    
- Acceptable risk
    

Therefore:

> **The metric is technical; choosing the metric is partly normative.**

---

# Statistical Fairness vs Ethical Fairness

|Dimension|Statistical Fairness|Ethical Fairness|
|---|---|---|
|Core Question|Are measurable outcomes or errors sufficiently balanced?|Is the treatment morally justified?|
|Nature|Quantitative|Normative + contextual|
|Main Tools|Metrics, tests, thresholds|Ethical reasoning, stakeholder analysis, impact analysis|
|Focus|Group-level or individual measurable behavior|Legitimacy of treatment and consequences|
|Evidence|Rates, errors, disparities|Metrics + context + rights + harms|
|Can Be Automated?|Partially|No, requires judgment|
|Main Risk|Choosing the wrong metric|Making vague judgments without evidence|
|Main Output|Measured disparity|Defensible ethical conclusion|

---

# Why Statistical Fairness Alone Is Insufficient

A system can satisfy a fairness metric while still being ethically problematic because:

- The target itself is biased
    
- The feature is ethically inappropriate
    
- Historical inequalities are reproduced
    
- The decision process lacks appeal
    
- The affected population was excluded from design
    
- Risks are imposed on one group while benefits go to another
    
- The model is used in an inappropriate context
    

Therefore:

> **Fairness metrics evaluate selected properties of a system, not the ethical legitimacy of the entire system.**

---

# Historical Data Example

Suppose a hiring model is trained on historical promotion decisions.

The historical dataset is statistically accurate.

But past promotion decisions may reflect:

- Gender discrimination
    
- Unequal access to leadership roles
    
- Biased manager evaluations
    
- Structural barriers
    

A model can faithfully learn the historical pattern.

Statistically:

> The model may be accurate.

Ethically:

> Reproducing that pattern may be unfair.

Therefore:

**Historical accuracy ≠ Ethical fairness**

---

# Proxy Variables

Suppose Gender is removed from a model.

However, the system still uses:

- Occupation
    
- Postal code
    
- Employment history
    
- Education history
    

These variables may indirectly encode information related to gender or socioeconomic status.

A statistical fairness audit may reveal outcome disparities.

Ethical fairness then asks:

> Is using these variables justified in this decision context?

Therefore:

**Proxy analysis is statistical**

but:

**Proxy legitimacy is ethical**

---

# Ethical Fairness Requires Context

The same disparity can have different ethical significance depending on the use case.

### Movie Recommendation

A 10% difference in recommendation exposure may create limited harm.

### Medical Diagnosis

A 10% difference in False Negative Rate may affect survival.

### Credit Approval

A persistent disparity may affect access to economic opportunity.

Therefore:

> **Fairness cannot be evaluated independently of consequence.**

---

# Fairness and Harm

A useful reasoning sequence is:

**Group**  
↓  
**Metric**  
↓  
**Disparity**  
↓  
**Cause**  
↓  
**Consequence**  
↓  
**Justification**

Do not stop at:

> “A disparity exists.”

Ask:

- Why does it exist?
    
- Is it avoidable?
    
- Who is harmed?
    
- How serious is the harm?
    
- Is the difference ethically justified?
    

---

# Fairness and Base Rates

Different groups may have different observed base rates.

This can make some statistical fairness criteria difficult or impossible to satisfy simultaneously.

Therefore:

> **Metric conflict is not necessarily a technical bug.**

It may reflect genuine tension between different definitions of fairness.

This means fairness governance must explicitly answer:

> Which fairness objective matters most in this context?

---

# When Fairness Metrics Conflict

Use this decision process:

### 1. Define the decision context

What decision is being made?

### 2. Identify affected groups

Who can be disadvantaged?

### 3. Identify the most harmful errors

Is False Positive or False Negative more serious?

### 4. Examine base rates and data quality

Are differences real, biased, or measurement artifacts?

### 5. Compare fairness criteria

Which criteria conflict?

### 6. Evaluate consequences

Who bears the harm under each option?

### 7. Select and justify the metric

Document why that fairness objective was prioritized.

### 8. Monitor after deployment

Fairness can change over time.

---

# Fairness as a Socio-Technical Property

Statistical fairness often focuses on the model.

Ethical fairness requires analysis of the broader system:

**Data → Model → Human → Process → Organization → Outcome**

Example:

A credit model may satisfy fairness thresholds.

But if rejected applicants:

- receive no explanation,
    
- cannot appeal,
    
- or are permanently excluded from future opportunities,
    

the broader process may still be ethically unfair.

Therefore:

> **A statistically fair model can operate inside an ethically unfair system.**

---

# Procedural Fairness

Ethical fairness also concerns **how decisions are made**, not only their statistical outcome.

Questions include:

- Was the process consistent?
    
- Was the person informed?
    
- Can the decision be challenged?
    
- Is there meaningful human review?
    
- Is correction possible?
    

This is sometimes called **procedural fairness**.

A system may therefore have statistically balanced outcomes but an unfair decision process.

---

# Outcome Fairness vs Process Fairness

### Outcome Fairness

> Are results distributed fairly?

### Process Fairness

> Was the decision-making process itself fair?

Both matter.

A model could produce balanced outcomes through an opaque and unchallengeable process.

That may still create ethical concerns.

---

# Fairness vs Justice

Statistical and ethical fairness still operate within a broader question of [[0150 Justice]].

A model may be ethically fair within a particular decision process while the surrounding social system remains unjust.

Therefore:

**Statistical Fairness**  
→ measures selected disparities

**Ethical Fairness**  
→ evaluates whether treatment is justified

**Justice**  
→ evaluates the broader distribution of rights, opportunities, benefits, harms, and power

---

# Example: Credit Approval

Suppose:

- Model A has slightly higher accuracy
    
- Model B reduces FNR disparity between groups
    
- Model B loses 1.5% overall accuracy
    

Statistical analysis tells us:

- How much performance changes
    
- How much disparity changes
    

It cannot by itself answer:

> Is the 1.5% performance loss worth the fairness improvement?

That requires ethical judgment based on:

- Severity of harm
    
- Number of affected people
    
- Reversibility
    
- Availability of alternatives
    
- Rights and opportunities at stake
    

This is where:

> **Statistical evidence becomes ethical judgment.**

---

# Practical Decision Framework

When evaluating fairness, ask:

1. **Which groups are affected?**
    
2. **Which fairness metric are we using?**
    
3. **Why is this metric appropriate?**
    
4. **What disparity exists?**
    
5. **What causes the disparity?**
    
6. **What harm results from it?**
    
7. **Is the difference justified?**
    
8. **Are there less harmful alternatives?**
    
9. **Who bears the cost of the chosen trade-off?**
    
10. **How will fairness be monitored over time?**
    

---

# Common Mistakes

### Mistake 1

> “The fairness metric passed, therefore the system is fair.”

False.

It only shows that one selected statistical criterion was satisfied.

---

### Mistake 2

> “All groups must receive identical outcomes.”

False.

Ethically relevant differences may justify different outcomes.

---

### Mistake 3

> “Fairness is subjective, so metrics are useless.”

False.

Metrics provide essential evidence, even though they cannot make the ethical decision alone.

---

### Mistake 4

> “The technically best fairness metric should determine the decision.”

False.

Fairness metric selection depends on context, consequences, and values.

---

### Mistake 5

> “A disparity automatically proves discrimination.”

Not necessarily.

A disparity is a signal that requires investigation, causal understanding, and ethical evaluation.

---

# Mental Model

**Statistical Fairness**

> **What disparity can we measure?**

↓

**Ethical Fairness**

> **Is that disparity justified?**

↓

**Ethical Decision**

> **What should we change, tolerate, or prohibit?**

---

## Stronger Mental Model

**Metric → Disparity → Cause → Harm → Justification → Decision**

Never stop at the metric.

---

# Key Takeaways

- **Statistical fairness makes disparities measurable.**
    
- **Ethical fairness determines whether those disparities are justified.**
    
- **A fairness metric is evidence, not an ethical conclusion.**
    
- **Choosing a fairness metric is itself partly a normative decision.**
    
- **Different fairness metrics can conflict.**
    
- **Equal Accuracy does not imply equal fairness.**
    
- **Different outcomes are not automatically unfair.**
    
- **A statistically fair model can exist within an ethically unfair socio-technical system.**
    
- **Fairness evaluation requires both quantitative evidence and contextual ethical judgment.**
    
- **The central question is not only “Are the numbers equal?” but “Are the differences ethically defensible?”**