## Core Distinction

**Fairness** asks:

> **Are people or groups being treated in an acceptably equitable way by this decision or system?**

**Justice** asks:

> **Is the broader distribution of rights, opportunities, benefits, harms, and power ethically defensible?**

A useful mental model is:

**Fairness = Equity within a decision process or outcome**

**Justice = The broader moral structure within which those decisions occur**

---

## Important Caveat

The terms **fairness** and **justice** overlap substantially in ethics and philosophy, and different traditions use them differently.

In AI Ethics, however, a practical distinction is useful:

- **Fairness** is often operationalized through measurable disparities in model behavior.
    
- **Justice** evaluates the wider social, institutional, historical, and political consequences of the AI system.
    

Therefore:

> **Fairness is often one component of justice, but justice is broader than fairness.**

---

# Fairness

Fairness focuses on whether individuals or groups are treated without **unjustified disadvantage**.

In AI systems, fairness questions often concern:

- Selection rates
    
- Approval rates
    
- Error rates
    
- Access to opportunities
    
- Treatment of similar individuals
    
- Performance across subgroups
    

Typical questions include:

- Does one group have a higher False Negative Rate?
    
- Are similarly qualified candidates treated similarly?
    
- Does the model systematically disadvantage a protected group?
    
- Are error rates acceptably distributed?
    

Fairness can therefore often be translated into:

**Principle → Metric → Threshold → Testing**

---

## Example: Credit Scoring

Suppose:

- Group A approval rate = 70%
    
- Group B approval rate = 50%
    

A fairness analysis asks:

- Why does this disparity exist?
    
- Are applicants similarly qualified?
    
- Are FPR/FNR different?
    
- Is a proxy variable influencing the model?
    
- Is the disparity justified by relevant risk factors?
    

This is primarily a **fairness problem**.

---

# Justice

Justice asks whether the **entire social arrangement** surrounding the AI system is ethically legitimate.

It goes beyond:

> “Does the model treat groups similarly?”

and asks:

- Who benefits from the system?
    
- Who bears the risks?
    
- Who has decision-making power?
    
- Who has historically been disadvantaged?
    
- Who can challenge the decision?
    
- Who has access to the benefits created by AI?
    
- Does the system reinforce existing structural inequality?
    
- Does it redistribute opportunities fairly?
    
- Are affected communities represented in governance?
    

Justice therefore evaluates:

**Outcomes + Rights + Power + History + Institutions + Social Structure**

---

## Example: Credit Scoring

Imagine the credit model passes all selected fairness tests.

However:

- low-income communities historically had less access to banking,
    
- those communities have thinner credit histories,
    
- the AI relies heavily on historical financial participation,
    
- rejected applicants have little opportunity to appeal,
    
- and the system further reduces their access to future credit.
    

The model may appear **fair under selected statistical metrics** while the overall system still reinforces structural disadvantage.

This becomes a **justice problem**.

---

# Fair Model ≠ Just System

This is the key distinction.

A model can satisfy a fairness metric while participating in an unjust system.

Example:

A hiring AI gives men and women equal error rates.

However, the organization:

- hires almost exclusively from elite universities,
    
- excludes applicants without unpaid internship experience,
    
- systematically disadvantages lower-income candidates,
    
- and provides no accessibility accommodations.
    

The AI may satisfy a narrow gender fairness criterion.

The **overall hiring system may still be unjust**.

Therefore:

> **Fairness analysis can be locally correct while justice analysis reveals a broader structural problem.**

---

# Justice Expands the Unit of Analysis

Fairness often evaluates:

**Model → Decision**

Justice evaluates:

**History → Data → Model → Institution → Decision → Social Consequence**

This connects directly to [[Socio-Technical Systems]].

Justice requires us to examine the whole system rather than only model outputs.

---

# Types of Fairness

## Group Fairness

Asks whether outcomes or errors differ unjustifiably between groups.

Examples:

- False Positive Rate
    
- False Negative Rate
    
- Selection Rate
    
- True Positive Rate
    
- Calibration
    

---

## Individual Fairness

A simplified principle:

> **Similar individuals should be treated similarly.**

The difficulty is defining:

> What counts as “similar”?

That itself can involve normative judgment.

---

## Procedural Fairness

Focuses on whether the **decision-making process** is fair.

Questions include:

- Can the person understand the process?
    
- Can they contest the decision?
    
- Is the same procedure consistently applied?
    
- Is there an appeal mechanism?
    

This connects fairness with:

- [[Transparency]]
    
- [[Explainability]]
    
- [[Contestability]]
    
- [[Accountability]]
    

---

# Dimensions of Justice

Justice is broader and can be divided into several useful dimensions.

## 1. Distributive Justice

Asks:

> **How are benefits, opportunities, costs, and harms distributed?**

Examples:

- Who gets access to loans?
    
- Who benefits from automation?
    
- Who loses employment opportunities?
    
- Who bears false-positive risk?
    

---

## 2. Procedural Justice

Asks:

> **Was the decision process legitimate and fair?**

Includes:

- Due process
    
- Transparency
    
- Appeal
    
- Consistency
    
- Participation
    

---

## 3. Corrective Justice

Asks:

> **What should happen after harm or wrongdoing occurs?**

Examples:

- Compensation
    
- Correction
    
- Appeal
    
- Remediation
    
- Model rollback
    

This connects to [[Redress]] and [[Incident Management]].

---

## 4. Recognitional Justice

Asks whether different groups are:

- properly recognized,
    
- respected,
    
- represented,
    
- and not reduced to stereotypes.
    

This matters when AI systems classify, profile, or represent people.

---

## 5. Structural Justice

Asks:

> **Does the system reinforce or challenge existing structural inequalities?**

Examples:

- Historical discrimination
    
- Unequal access to education
    
- Unequal access to credit
    
- Wealth inequality
    
- Digital exclusion
    

This dimension is especially important because:

> **Historical data may encode structurally unjust conditions even when the data is statistically accurate.**

---

# Historical Bias and Justice

Suppose historical hiring data shows that most senior managers were men.

A predictive model may accurately learn:

> Certain male-associated career patterns correlate with promotion.

From a purely predictive perspective, the model may be correct.

From a justice perspective, however, we must ask:

> Does this historical pattern reflect merit, or historical inequality?

Therefore:

**Historical accuracy ≠ Ethical legitimacy**

This is one reason why simply learning from historical data can reproduce injustice.

---

# Fairness Metrics Do Not Define Justice

Metrics such as:

- Demographic Parity
    
- Equal Opportunity
    
- Equalized Odds
    
- Calibration
    

can help analyze fairness.

But they cannot determine by themselves:

- Which groups deserve protection
    
- What outcome should be prioritized
    
- What level of inequality is justified
    
- Which historical inequalities should be corrected
    
- How benefits and risks should be distributed
    
- Whether the system should exist at all
    

Those are **normative questions**.

Therefore:

> **Fairness metrics provide evidence; they do not replace ethical judgment.**

---

# Example: Healthcare AI

Suppose a diagnostic model has equal sensitivity across ethnic groups.

From a fairness perspective:

> This may be a positive result.

But justice asks additional questions:

- Do all groups have equal access to the AI system?
    
- Do disadvantaged communities have access to follow-up treatment?
    
- Was the model validated on underserved populations?
    
- Who benefits financially from the technology?
    
- Does deployment increase or reduce healthcare inequality?
    

The model may be fair.

The healthcare system may still be unjust.

---

# Example: Industrial Automation

An AI system optimizes maintenance and reduces downtime by 25%.

The model treats all equipment sites consistently.

Fairness may not be the primary issue.

Justice questions may include:

- Are workers displaced by automation?
    
- Are productivity gains shared with workers?
    
- Are safety risks transferred to frontline technicians?
    
- Were workers involved in the deployment decision?
    
- Does management receive the benefits while operators carry the risk?
    

Justice therefore extends beyond protected-group fairness.

---

# Fairness vs Equality

These concepts should also be separated.

**Equality** often means:

> Everyone receives the same treatment or resource.

**Fairness / Equity** may require:

> Different treatment when relevant differences justify it.

Example:

Giving every patient exactly the same treatment is equal.

Giving patients treatment based on medically relevant needs may be fairer.

Therefore:

**Equality ≠ Fairness**

---

# Fairness vs Justice vs Equality

|Concept|Core Question|
|---|---|
|**Equality**|Is everyone treated the same?|
|**Fairness**|Are differences in treatment justified and equitable?|
|**Justice**|Is the broader distribution of rights, opportunities, harms, and power defensible?|

---

# Fairness in AI Engineering

Fairness is often operationalized through:

**Protected Groups**  
↓  
**Fairness Objective**  
↓  
**Metric**  
↓  
**Threshold**  
↓  
**Testing**  
↓  
**Mitigation**  
↓  
**Monitoring**

Example:

**Fairness Principle**  
↓  
Avoid unjustified disparity in missed diagnoses  
↓  
Measure subgroup FNR  
↓  
Define acceptable disparity  
↓  
Validate model  
↓  
Mitigate if threshold is exceeded  
↓  
Monitor after deployment

---

# Justice in AI Governance

Justice requires broader governance questions:

**Stakeholders**  
↓  
Who benefits and who bears risk?

**History**  
↓  
What existing inequalities affect the system?

**Power**  
↓  
Who controls design and deployment?

**Participation**  
↓  
Who has a voice?

**Rights**  
↓  
What claims do affected people have?

**Distribution**  
↓  
How are benefits and harms allocated?

**Redress**  
↓  
What happens when harm occurs?

---

# Paradoxical Example

Suppose a loan model satisfies Equal Opportunity.

However:

- the bank serves only wealthy neighborhoods,
    
- lower-income communities lack access to branches,
    
- rejected applicants cannot appeal,
    
- and the system relies on historical financial participation.
    

Question:

> Is the model fair?

Possibly, under the selected fairness metric.

Question:

> Is the overall system just?

Not necessarily.

This demonstrates:

> **Fairness can be evaluated locally; justice requires system-level analysis.**

---

# Key Decision Questions

## Fairness Questions

- Are outcomes different across groups?
    
- Are error rates different?
    
- Are similar people treated similarly?
    
- Are disparities justified?
    
- Which fairness metric fits the context?
    

## Justice Questions

- Who benefits?
    
- Who bears the harm?
    
- Who has power?
    
- Who lacks representation?
    
- What historical inequalities matter?
    
- Can affected people challenge decisions?
    
- Are benefits and risks distributed legitimately?
    
- Does the system reinforce structural disadvantage?
    
- Should this system exist in its current form at all?
    

---

# Connection to Socio-Technical Systems

Fairness can sometimes be assessed at the model level.

Justice almost always requires a broader [[Socio-Technical Systems]] perspective.

The appropriate unit of analysis becomes:

**Data + Model + Humans + Organization + Institutions + Society**

not merely:

**Model + Metrics**

---

# Connection to Responsible AI

A useful distinction is:

**AI Ethics**  
→ Defines fairness and justice as values.

**Responsible AI**  
→ Creates processes for evaluating and mitigating relevant risks.

**AI Governance**  
→ Determines who has authority to make and review decisions.

**Fairness Testing**  
→ Provides technical evidence.

**Justice Analysis**  
→ Evaluates the broader legitimacy and distributional consequences of the system.

---

# Common Mistakes

### Mistake 1

> “The model passed fairness metrics, therefore the system is just.”

False.

Fairness metrics evaluate selected dimensions of model behavior, not the entire social system.

---

### Mistake 2

> “Fairness means everyone gets the same outcome.”

False.

Fairness depends on context and justified differences.

---

### Mistake 3

> “Justice is just another fairness metric.”

False.

Justice includes power, rights, history, institutions, participation, and distribution of benefits and harms.

---

### Mistake 4

> “If historical data is accurate, using it is fair.”

Not necessarily.

Historical data can accurately represent an unjust historical system.

---

# Mental Model

**Equality**  
→ Are people treated the same?

**Fairness**  
→ Are differences in treatment justified?

**Justice**  
→ Is the overall system of rights, opportunities, harms, benefits, and power defensible?

Or more compactly:

**Fairness = Is this decision equitable?**

**Justice = Is this system equitable and legitimate?**

---

# Key Takeaways

- **Fairness and justice overlap, but justice is usually broader.**
    
- **Fairness often focuses on decisions, outcomes, opportunities, and error distributions.**
    
- **Justice includes rights, power, history, institutions, participation, and structural inequality.**
    
- **A model can be statistically fair while participating in an unjust socio-technical system.**
    
- **Fairness metrics are tools for evidence, not complete definitions of justice.**
    
- **Historical accuracy does not guarantee ethical legitimacy.**
    
- **Justice requires stakeholder and power analysis, not only model evaluation.**
    
- **Fairness asks whether differences are justified; justice asks whether the broader system is defensible.**
    

---
