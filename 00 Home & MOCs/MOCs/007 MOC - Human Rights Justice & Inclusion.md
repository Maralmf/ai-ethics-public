---
type: moc
status: mature
domains:
  - human-rights-justice
created: 2026-09-01
updated: 2026-09-25
---

# Human Rights, Justice & Inclusion

## Scope

This MOC organizes concepts concerning human rights, dignity, justice, equality, non-discrimination, inclusion, accessibility, participation, and vulnerability in the ethical evaluation of AI systems.

Its central concern is not merely whether an AI system performs similarly across populations, but whether the system respects relevant rights and human dignity, distributes benefits and burdens justifiably, and avoids creating or reinforcing unjust forms of exclusion, discrimination, or disadvantage.

The central questions are:

> **Whose rights, opportunities, interests, freedoms, and forms of agency are affected by the AI system?**

and:

> **Are the benefits, burdens, risks, errors, and decision-making powers distributed in a way that can be ethically justified?**

---

## Why This Domain Matters

AI systems can influence access to:

- employment
- education
- healthcare
- financial services
- insurance
- housing
- public benefits
- policing and criminal justice
- information
- political participation
- digital services

In these contexts, ethical evaluation cannot be reduced to model accuracy.

A technically effective system may still:

- discriminate
- undermine human dignity
- restrict autonomy
- exclude vulnerable groups
- reproduce structural disadvantage
- distribute errors unfairly
- make essential services less accessible
- weaken opportunities for participation or redress

Therefore:

> Ethical evaluation must consider not only what an AI system predicts, but also how it affects rights, opportunities, relationships, institutions, and distributions of power.

---

# Conceptual Orientation

A useful working relationship is:

**Human Dignity**

↓

**Human Rights**

↓

**Justice**

↓

**Equality / Equity / Non-Discrimination**

↓

**Inclusion & Accessibility**

↓

**Requirements for AI Design, Deployment, and Governance**

This is a conceptual orientation rather than a universal hierarchy or a claim of derivation.

The concepts overlap, and different ethical, legal, philosophical, and political traditions may justify or organize them differently. Human dignity, rights, justice, equality, non-discrimination, inclusion, and accessibility should therefore be treated as related but non-interchangeable concepts.

---

# Human Dignity

- Human Dignity

Human dignity concerns the moral status and inherent worth attributed to persons.

In AI Ethics, dignity-related concerns may arise when systems:

- reduce individuals to data profiles
- treat people merely as means to institutional objectives
- subject individuals to degrading or dehumanizing treatment
- make consequential decisions without meaningful recognition of individual circumstances
- undermine agency or personhood

### Key Question

> Does the AI-enabled process treat affected people as persons with legitimate claims, rights, and agency rather than merely as objects of prediction or optimization?

### Important Distinction

Respect for dignity cannot generally be established by a single technical metric.

---

# Human Rights

- Human Rights

Human rights provide an important normative framework and, where applicable, a legal framework for evaluating AI systems.

The precise content, scope, and enforceability of particular rights can vary across legal instruments and jurisdictions. Ethical human-rights reasoning and positive-law analysis should therefore be distinguished rather than treated as identical.

Relevant rights may include:

- Right to Privacy
- Freedom of Expression
- Freedom of Association
- Right to Equality
- Non-Discrimination
- Right to an Effective Remedy
- Due Process
- Access to Information
- Human Autonomy

Depending on the context, AI systems may also affect rights associated with:

- work
- education
- health
- social protection
- political participation
- access to essential services

### Key Question

> Which rights may be enabled, restricted, burdened, or placed at risk by this system?

---

## Rights Are Not Identical to Interests

A useful distinction is:

**Interest**

→ something that matters to a stakeholder

**Right**

→ a claim that may impose corresponding duties or constraints on others

Not every stakeholder preference constitutes a right.

Conversely, a rights-based constraint may remain relevant even when violating it would improve aggregate performance or efficiency.

Related:

- Rights vs Interests
- Rights-Based Ethics

---

# Justice

- Justice

Justice concerns how benefits, burdens, rights, opportunities, recognition, institutional arrangements, and decision-making procedures should be structured and evaluated.

Justice is broader than statistical fairness.

Important perspectives include:

- Distributive Justice
- Procedural Justice
- Corrective Justice
- Restorative Justice
- Recognitional Justice

---

## Distributive Justice

- Distributive Justice

Core question:

> How are benefits, opportunities, harms, risks, and resources distributed?

Relevant AI examples:

- allocation of healthcare resources
- credit approval
- employment opportunities
- access to public services
- distribution of false-positive and false-negative errors

---

## Procedural Justice

- Procedural Justice

Core question:

> Is the decision-making process itself fair and legitimate?

Relevant considerations include:

- transparency
- consistency
- participation
- impartiality
- ability to contest decisions
- access to review
- explanation
- appropriate human oversight

Related:

- Contestability
- Redress
- Human Oversight

---

## Recognitional Justice

- Recognitional Justice

Core question:

> Are individuals and groups represented, understood, and treated in ways that respect their identities and social circumstances?

AI systems may create recognitional injustice through:

- stereotyping
- erasure
- misclassification
- degrading representation
- systematic under-recognition of particular communities

Related:

- Representational Harm
- Group Harm

---

# Equality

- Equality

Equality concerns the treatment or status of persons according to a relevant conception of equal moral standing.

However, equality does not necessarily require identical treatment in every context.

A central distinction is:

## Formal Equality

- Formal Equality

> Treat similarly situated individuals in the same way.

versus:

## Substantive Equality

- Substantive Equality

> Consider whether apparently identical rules reproduce or reinforce existing disadvantage.

This distinction is important in AI because:

> identical model treatment does not necessarily produce equitable or just outcomes.

---

# Equity

- Equity

Equity recognizes that achieving substantively fair conditions may require attention to different needs, disadvantages, starting positions, or barriers.

Therefore:

**Equality**

does not always mean:

**identical intervention**

and:

**different treatment**

does not automatically imply:

**unjust discrimination**

### Key Question

> Does treating everyone identically preserve an existing structural disadvantage?

Related:

- Equality vs Equity
- Substantive Equality

---

# Non-Discrimination

- Non-Discrimination

Non-discrimination concerns unjustified disadvantage associated with protected or otherwise ethically salient characteristics. Its precise legal meaning, protected grounds, tests, exceptions, and remedies vary by jurisdiction; ethical analysis may also identify concerns that extend beyond legally protected categories.

Potentially relevant characteristics may include, depending on jurisdiction and context:

- sex
- race or ethnicity
- disability
- age
- religion
- nationality
- sexual orientation
- socioeconomic position

AI-related discrimination may arise even when a protected attribute is not explicitly included in the model.

Related:

- Proxy Bias
- Historical Bias
- Representation Bias
- Algorithmic Bias

---

## Direct and Indirect Discrimination

### Direct Discrimination

- Direct Discrimination

In general terms, direct discrimination concerns less favorable treatment explicitly connected to a protected characteristic, subject to the definitions and conditions of the applicable legal framework.

### Indirect Discrimination

- Indirect Discrimination

In general terms, indirect discrimination concerns an apparently neutral rule, criterion, or practice that places a protected group at a particular disadvantage, again subject to the applicable legal framework and any recognized justification tests.

This distinction is especially important in AI because:

> apparently neutral variables and decision rules can still produce systematically unequal effects.

---

# Fairness and Justice

- Fairness
- Justice

These concepts should not be treated as synonyms.

A useful working distinction is:

**Fairness**

→ concerns whether treatment, procedures, outcomes, or error distributions satisfy a justified conception of fairness.

**Justice**

→ concerns the broader normative structure within which benefits, burdens, rights, opportunities, institutions, and social relationships are evaluated.

Therefore:

> Satisfying a statistical fairness criterion does not by itself establish that an AI system is just.

For example, a system could satisfy a chosen parity metric while:

- being deployed for an illegitimate purpose
- using an unjust target variable
- reinforcing structural disadvantage
- violating privacy
- denying meaningful contestability

Related:

→ 009 MOC - Bias & Fairness

---

# Inclusion

- Inclusion

Inclusion concerns whether people and groups are able to participate in, benefit from, and influence systems that affect them.

In AI systems, exclusion may occur through:

- inaccessible interfaces
- language barriers
- missing population groups
- inappropriate assumptions about users
- inability to opt out
- absence of stakeholder participation
- digital access barriers
- lack of accommodation for disability

### Key Question

> Who is systematically unable to access, use, understand, influence, or benefit from this system?

---

# Accessibility

- Accessibility

Accessibility concerns whether systems can be effectively used by people with diverse abilities, needs, and circumstances.

Accessibility should not be treated merely as interface convenience.

In consequential AI systems, inadequate accessibility may affect:

- participation
- access to services
- ability to understand decisions
- ability to contest decisions
- meaningful exercise of rights

Related:

- Disability Inclusion
- Universal Design
- Inclusive Design

---

# Inclusion Is Not Automatically Ethical

An important caveat:

> Inclusion in an ethically problematic system does not necessarily make the system ethically acceptable.

For example, increasing demographic representation in a system used for unjustified mass surveillance would not by itself resolve the underlying ethical problem.

Therefore:

**better inclusion**

does not automatically imply:

**ethical legitimacy**

The purpose and institutional context of the system must also be evaluated.

---

# Vulnerability

- Vulnerability

Some individuals or groups may face greater exposure to harm or have less ability to avoid, understand, challenge, or recover from AI-mediated decisions.

Sources of vulnerability may include:

- economic dependency
- disability
- limited digital literacy
- immigration status
- age
- institutional dependency
- lack of bargaining power
- limited access to legal or technical expertise

Vulnerability should not be understood only as an inherent or fixed characteristic of individuals or groups.

It may also be relational, situational, or structurally produced:

> **Vulnerability can be created or intensified by institutional arrangements, dependencies, power asymmetries, and technological systems.**

Related:

- Power Asymmetry
- Institutional Vulnerability
- 008 MOC - Harm Risk & Power

---

# Participation

- Stakeholder Participation
- Participatory AI

Affected communities may possess knowledge that is unavailable to:

- model developers
- managers
- auditors
- regulators

Participation can therefore contribute to:

- problem formulation
- harm identification
- requirement definition
- evaluation
- contextual understanding
- legitimacy

However, these benefits depend on how participation is structured and whether participants have meaningful influence.

However:

> participation should not automatically be treated as evidence that a system is ethical.

Important questions include:

- Who participated?
- At what stage?
- With what authority?
- Were dissenting views represented?
- Could participants materially change the decision?

---

# Structural and Historical Context

AI systems operate within existing social and institutional structures.

Observed disparities may therefore reflect:

- historical discrimination
- unequal access to resources
- institutional practices
- previous policy decisions
- structural inequality

Related:

- Structural Inequality
- Historical Bias
- Institutional Bias

A key reasoning chain is:

**Historical / Structural Conditions**

↓

**Data-Generating Process**

↓

**Observed Data**

↓

**Model**

↓

**Decision Policy**

↓

**Allocation of Benefits and Harms**

↓

**Potential Reinforcement of Existing Inequality**

Therefore:

> Removing a protected attribute from a model does not necessarily remove the influence of historical or structural inequality.

---

# Key Distinctions

This domain requires several distinctions to remain explicit.

### Fairness vs Justice

Statistical or procedural fairness does not exhaust broader questions of justice.

### Equality vs Equity

Equal treatment and equitable treatment are not always identical.

### Formal vs Substantive Equality

An apparently neutral rule may preserve existing disadvantage.

### Direct vs Indirect Discrimination

Discrimination may arise without explicit use of a protected characteristic.

### Inclusion vs Accessibility

Inclusion concerns meaningful participation and belonging; accessibility concerns whether participation is practically possible.

### Rights vs Interests

Rights may impose stronger normative constraints than ordinary stakeholder preferences.

### Legal Rights vs Ethical Claims

Legal recognition and ethical justification overlap but are not identical.

### Fairness vs Non-Discrimination

Statistical fairness criteria and legal or ethical non-discrimination requirements should not automatically be treated as equivalent.

---

# Relationship to Bias & Fairness

This MOC and 009 MOC - Bias & Fairness address related but different questions.

## Human Rights, Justice & Inclusion

asks:

> What constitutes just, rights-respecting, and inclusive treatment?

## Bias & Fairness

asks:

> Where can systematic disparities arise, how can they be measured, and which fairness criteria may be relevant?

A useful relationship is:

**Rights / Justice**

↓

**Normative Fairness Concern**

↓

**Operational Fairness Criterion**

↓

**Metric**

↓

**Evidence**

↓

**Ethical Interpretation**

The arrow should not be reversed automatically.

> A metric should operationalize a justified normative concern; the metric itself should not define what justice means.

---

# Relationship to Harm & Power

→ 008 MOC - Harm Risk & Power

Rights violations and injustices often involve:

- harm
- vulnerability
- dependency
- institutional power
- unequal ability to contest decisions

A disparity becomes ethically more significant when combined with:

**high consequence**

+

**low individual power**

+

**limited contestability**

+

**historical disadvantage**

---

# Relationship to Accountability

→ 014 MOC - Accountability Contestability & Redress

Rights are difficult to protect without institutional mechanisms for:

- answerability
- contestability
- review
- correction
- remedy

A formally recognized right may provide weak practical protection when affected people lack realistic mechanisms for exercising, contesting, or enforcing it.

---

# Relationship to Governance

→ 018 MOC - Governance Regulation & Legitimacy

Human-rights and justice concerns may inform:

- AI impact assessment
- governance requirements
- deployment restrictions
- documentation
- audit criteria
- stakeholder participation
- redress mechanisms

Legal compliance and ethical legitimacy should nevertheless remain distinct.

A system can comply with applicable law while still raising unresolved ethical questions, and ethical concerns should not be presented as legal violations unless the relevant legal analysis supports that conclusion.

---

# Practical Evaluation Lens

When evaluating an AI system, ask:

## Rights

- Which rights may be affected?
- Is interference with those rights justified?
- Are less intrusive alternatives available?

## Justice

- Who receives the benefits?
- Who bears the burdens?
- Which groups experience the most consequential errors?

## Equality

- Are similarly situated individuals treated consistently?
- Could identical treatment reproduce existing disadvantage?

## Non-Discrimination

- Are particular groups systematically disadvantaged?
- Could apparently neutral variables function as proxies?

## Inclusion

- Who was represented in system design and evaluation?
- Who is unable to participate or benefit?

## Accessibility

- Can affected people meaningfully use, understand, and challenge the system?

## Vulnerability

- Who has the least power to refuse, avoid, or recover from the decision?

## Power

- Who defines the problem?
- Who sets the thresholds?
- Who can override the system?
- Who can contest the outcome?

---

# Example — AI-Assisted Hiring

Consider an AI system used to rank job applicants.

A narrow evaluation might ask:

> Is model accuracy high?

A human-rights and justice analysis asks additional questions.

### Equality

Are similarly qualified applicants treated differently?

### Non-Discrimination

Do protected or historically disadvantaged groups experience systematic disadvantage?

### Substantive Justice

Does the target variable reproduce historical hiring preferences rather than legitimate job-related merit?

### Inclusion

Were relevant applicant populations represented during development and evaluation?

### Accessibility

Can applicants with disabilities meaningfully participate in the assessment process?

### Procedural Justice

Can applicants understand and challenge consequential errors?

### Power

Does the employer possess substantially more information and decision-making authority than affected applicants?

### Redress

Can an incorrect decision be corrected?

This demonstrates why:

> **Fairness metrics can be necessary analytical tools in some contexts, but they are not a complete theory of justice.**

---

# Common Failure Modes in Ethical Reasoning

### "Equal treatment is always fair."

Not necessarily.

→ Equality vs Equity

---

### "Removing protected attributes prevents discrimination."

Not necessarily.

→ Proxy Bias

---

### "A fairness metric proves that a system is just."

False.

→ Fairness vs Justice

---

### "More representative AI is necessarily ethical AI."

False.

Representation does not justify an ethically illegitimate purpose.

---

### "Compliance with anti-discrimination law settles the ethical question."

Not necessarily.

Legal compliance and ethical legitimacy are related but distinct.

→ Legal vs Ethical vs Legitimate

---

### "Vulnerability is simply a fixed property of certain groups."

Too simplistic.

Vulnerability can be produced or intensified by systems, institutions, and power relations.

---

# Ethical Reasoning Chain

A useful reasoning sequence is:

**Who is affected?**

↓

**Which rights, interests, and opportunities are at stake?**

↓

**What harms or disadvantages are possible?**

↓

**How are power and vulnerability distributed?**

↓

**What conception of justice is relevant?**

↓

**What equality or non-discrimination requirements follow?**

↓

**How can those requirements be operationalized?**

↓

**What evidence is needed?**

↓

**What residual injustice or risk remains?**

↓

**Who has authority to accept, mitigate, or reject it?**

---

# Related MOCs

### Foundations
→ 006 MOC - Foundations & Ethical Theory

### Harm, Risk & Power
→ 008 MOC - Harm Risk & Power

### Bias & Fairness
→ 009 MOC - Bias & Fairness

### Privacy & Data Governance
→ 010 MOC - Privacy & Data Governance

### Human Agency
→ 012 MOC - Human Agency Autonomy & Oversight

### Accountability
→ 014 MOC - Accountability Contestability & Redress

### Ethical Reasoning
→ 017 MOC - Ethical Trade-offs & Decision Reasoning

### Governance
→ 018 MOC - Governance Regulation & Legitimacy

---

# Evidence & Normative Status

Claims in this domain may have different epistemic and normative status.

Distinguish among:

- **empirical claims** — what disparities, outcomes, access barriers, or participation patterns are observed
- **causal claims** — what mechanisms are proposed to explain those observations
- **normative claims** — what treatment, distribution, or institutional arrangement ought to be considered justifiable
- **legal claims** — what applicable law requires, permits, prohibits, or remedies in a particular jurisdiction

These categories interact but should not be collapsed.

For example:

**Observed group disparity**

↓

may justify further investigation

but does not automatically establish:

**causal discrimination**

or:

**ethical injustice**

or:

**legal discrimination**

Each conclusion may require additional evidence and a distinct form of justification.

---

# Evidence & Literature Directions

## Human Rights Foundations

- Universal human rights instruments
- international human-rights guidance relevant to AI
- rights-based approaches to technology governance

## Justice

- distributive justice
- procedural justice
- theories of equality and equity
- recognition and structural injustice

## Algorithmic Justice

- algorithmic discrimination
- structural inequality and automated decision-making
- fairness and non-discrimination
- disability and accessibility in AI

## Participation & Inclusion

- participatory approaches to AI
- inclusive design
- affected-community engagement

Specific sources should be maintained as dedicated literature or framework notes and linked to the relevant concepts.

---

# Open Questions

- Can statistical fairness adequately represent substantive justice?
- When is differential treatment ethically justified?
- How should historical disadvantage affect present AI decision rules?
- When should individual rights constrain aggregate social benefit?
- Which rights should be treated as non-negotiable constraints?
- How should conflicts among rights be resolved?
- Who should define what counts as a relevant protected or vulnerable group?
- How granular should intersectional analysis become before statistical uncertainty becomes prohibitive?
- Can meaningful inclusion exist without decision-making power?
- When is stakeholder participation genuinely influential rather than symbolic?
- How should AI systems account for structural injustice without reinforcing essentialist group categories?
- When should rights or justice concerns lead to non-deployment rather than mitigation?

---

## Continue Exploring

→ 008 MOC - Harm Risk & Power

→ 009 MOC - Bias & Fairness

→ 012 MOC - Human Agency Autonomy & Oversight

→ 014 MOC - Accountability Contestability & Redress

→ 017 MOC - Ethical Trade-offs & Decision Reasoning

→ 018 MOC - Governance Regulation & Legitimacy
