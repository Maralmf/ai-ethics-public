---
type: moc
status: mature
domains:
  - foundations
created: 2026-09-01
updated: 2026-09-25
---

# Foundations & Ethical Theory

## Scope

This MOC organizes the conceptual and normative foundations of AI Ethics.

It connects ethical theories, human values, ethical principles, socio-technical perspectives, responsibility, and foundational distinctions needed to evaluate AI systems beyond technical performance.

The central question is:

> **What ought humans, organizations, and institutions do when designing, developing, deploying, using, monitoring, and governing AI systems?**

---

## Orientation

AI Ethics is not primarily concerned with whether an AI system can perform a task.

It also asks whether:

- the purpose is ethically legitimate
- AI should be used for the task at all
- relevant rights and values are respected
- benefits, burdens, opportunities, and harms are distributed justifiably
- human agency and autonomy are preserved
- responsibility and accountability can be assigned
- affected stakeholders can challenge decisions and seek redress
- remaining risks can be ethically justified
- deployment remains acceptable as the system and its context change

Start with:

→ [002 What is AI Ethics](./002%20What%20is%20AI%20Ethics.md)

---

# Core Concepts

- [002 What is AI Ethics](./002%20What%20is%20AI%20Ethics.md)
- Ethical AI
- Responsible AI
- Trustworthy AI
- AI Non-Neutrality
- Socio-Technical Systems
- Human Values
- Ethical Principles
- Normative Ethics
- Applied Ethics
- Technology Ethics

---

# Foundational Relationship

A useful working distinction is:

### AI Ethics

Primary question:

> **What ought we do regarding AI?**

Focus:

- values
- rights
- duties
- harms
- justice
- legitimacy
- ethical justification

### Responsible AI

Primary question:

> **How should ethical and societal responsibilities be operationalized?**

Focus:

- requirements
- processes
- controls
- documentation
- audits
- governance
- monitoring

### Trustworthy AI

Primary question:

> **What properties, processes, and evidence justify appropriate reliance on an AI system?**

Focus may include:

- reliability
- safety
- robustness
- fairness
- transparency
- privacy
- accountability
- assurance evidence

### Ethical AI

Primary question:

> **Can this AI system, its intended use, and its surrounding socio-technical arrangements be ethically justified?**

Ethical AI is best treated here as an aspirational characterization rather than a binary technical property.

---

## Important Terminological Caution

[002 What is AI Ethics](./002%20What%20is%20AI%20Ethics.md), Responsible AI, Trustworthy AI, and Ethical AI overlap, but they should not be treated as synonyms.

Their boundaries are not universally standardized across academic, policy, standards, and industry literature.

A useful working distinction in this knowledge base is:

**AI Ethics**  
→ normative inquiry

**Responsible AI**  
→ operationalization of responsibilities

**Trustworthy AI**  
→ conditions and evidence supporting justified reliance

**Ethical AI**  
→ aspiration toward ethically justifiable AI design, use, and governance

These are working distinctions for this knowledge base, not claims of universal terminology.

---

# Key Distinctions

- AI Ethics vs Ethical AI
- AI Ethics vs Responsible AI
- Responsible AI vs Trustworthy AI
- Ethics vs Law
- Legal vs Ethical vs Legitimate
- Descriptive vs Normative Claims
- Values vs Principles
- Principles vs Requirements
- Explanation vs Justification
- Moral Agency vs Moral Responsibility

---

# Ethical Theories & Traditions

AI Ethics draws on multiple normative traditions rather than a single universally decisive ethical theory.

## Consequentialist Approaches

- Consequentialism
- Utilitarianism

Core question:

> **What benefits, harms, and broader consequences result from the system and its use?**

Related:

- Beneficence
- Non-Maleficence
- Harm

---

## Deontological and Rights-Based Approaches

- Deontology
- Rights-Based Ethics
- Human Rights
- Human Dignity

Core question:

> **What duties, rights, or constraints should apply even when violating them might increase aggregate benefit?**

---

## Justice-Oriented Approaches

- Justice
- Distributive Justice
- Procedural Justice
- Equality
- Equity
- Non-Discrimination

Core question:

> **How are benefits, burdens, opportunities, errors, risks, and decision-making power distributed?**

---

## Virtue and Care-Oriented Approaches

- Virtue Ethics
- Care Ethics

Core questions:

> **What forms of responsible professional conduct should guide AI development and deployment?**

> **How should dependency, vulnerability, relationships, context, and care shape ethical evaluation?**

---

# Human Values & Normative Commitments

Relevant values and normative commitments may include:

- Human Dignity
- Human Autonomy
- Justice
- Fairness
- Privacy
- Safety
- Freedom
- Solidarity
- Accountability
- Sustainability

Values and normative commitments may:

- support one another
- overlap
- conflict
- require contextual interpretation
- imply different operational requirements in different contexts

Therefore:

> **Values should not be translated directly into metrics without an explicit reasoning and justification step.**

---

# Ethical Principles

Ethical principles provide more action-guiding expressions of values and normative commitments.

Examples may include:

- Beneficence
- Non-Maleficence
- respect for autonomy
- justice
- non-discrimination
- privacy protection
- accountability
- proportionality
- precaution

A principle is not yet an operational requirement.

For example:

> **Respect human autonomy**

does not by itself specify:

- what authority humans must retain
- which decisions require review
- what information reviewers need
- when automation must defer
- what evidence demonstrates adequate control

This is why principles require further operationalization.

---

# From Values to Requirements

A central translation problem in Responsible AI is:

**Human Value / Right**

↓

**Ethical Principle**

↓

**Ethical Requirement**

↓

**Operational Criterion**

↓

**Metric / Evaluation Method / Evidence Requirement**

↓

**Acceptance Criterion / Threshold / Decision Rule**

↓

**Technical or Organizational Control**

↓

**Verification / Assurance Evidence**

↓

**Residual Risk**

↓

**Governance Decision**

↓

**Deployment Conditions**

↓

**Monitoring Indicator**

↓

**Trigger / Escalation / Stop Criterion**

↓

**Reassessment**

Related:

→ 019 MOC - Responsible AI Engineering & Assurance

→ 020 MOC - Lifecycle Monitoring & Incident Management

This chain is not a claim that ethics can be reduced to metrics.

Each translation introduces assumptions that may require empirical evidence, normative justification, and governance judgment.

---

# Empirical, Causal & Normative Reasoning

AI Ethics requires distinguishing among empirical observations, causal explanations, and normative conclusions.

### Empirical Claim

> Group A experiences a higher false-positive rate than Group B.

This describes an observed disparity.

### Causal Question

> What mechanisms produced the disparity?

Possible explanations may involve:

- historical conditions
- selection
- measurement
- labels
- institutional practices
- model design
- thresholds
- deployment conditions

### Normative Question

> Is the disparity unjust, discriminatory, or ethically unacceptable?

Answering the normative question may require additional reasoning concerning:

- harm
- context
- historical disadvantage
- rights
- available alternatives
- uncertainty
- stakeholder interests
- legitimacy

Therefore:

> **Empirical evidence can inform ethical judgment, but it does not by itself determine what ought to be done.**

and:

> **Causal explanation and ethical justification remain distinct tasks.**

Related:

- Descriptive vs Normative Claims
- Fairness
- Justice

---

# AI Non-Neutrality

AI systems embody choices about:

- which problems are considered worth solving
- whether AI is an appropriate intervention
- how targets are defined
- what data are collected
- which variables are measured
- what outcomes count as success
- which errors are prioritized
- what thresholds are used
- who receives decision-making authority
- which stakeholders are consulted
- what risks are considered acceptable

These choices may encode normative assumptions.

This does not mean that every technical decision is arbitrary or intentionally ideological.

It means that technical systems are designed and deployed within social, institutional, and normative contexts.

Related:

- AI Non-Neutrality
- Problem Formulation
- Value-Laden Design

---

# Socio-Technical Perspective

Ethical evaluation should not focus only on the algorithm.

An AI-enabled decision system may include:

**Historical & Social Context**

↓

**Institutional Objectives**

↓

**Problem Formulation**

↓

**Data Generation**

↓

**Measurement & Labels**

↓

**Model**

↓

**Decision Policy**

↓

**Human Interpretation**

↓

**Organizational Action**

↓

**Social Consequences**

Therefore:

> **Ethical evaluation should consider the entire socio-technical decision system rather than treating model behavior as the sole source of ethical outcomes.**

Related:

- Socio-Technical Systems
- Power Asymmetry
- Information Asymmetry
- Institutional Context

---

# Moral Agency & Responsibility

An important foundational distinction concerns whether AI systems themselves should be treated as moral agents.

Relevant concepts:

- Moral Agency
- Moral Responsibility
- Human Responsibility
- Responsibility Gap
- Many Hands Problem

### Working Principle

Current AI systems should not automatically be treated as independent moral agents merely because they produce autonomous, adaptive, or complex behavior.

Ethical and institutional responsibility typically remains distributed among:

- developers
- deployers
- organizations
- operators
- decision-makers
- procurers
- regulators
- other relevant actors

The precise distribution of responsibility depends on context, authority, control, knowledge, role, and institutional arrangements.

Related:

- Accountability vs Responsibility
- 014 MOC - Accountability Contestability & Redress

---

# Ethical Acceptability

Ethical acceptability should not be inferred from success on a single dimension.

An AI system may be:

- fair according to one criterion but unsafe
- reliable but excessively intrusive
- transparent but discriminatory
- privacy-preserving but socially harmful
- legally compliant but ethically questionable

Ethical acceptability is therefore:

- contextual
- multi-dimensional
- evidence-informed
- normatively reasoned
- sensitive to affected stakeholders
- subject to reassessment over time

Therefore:

> **No single metric, audit, assessment, framework, standard, regulation, or certification is sufficient on its own to establish the overall ethical acceptability of an AI system or its use.**

Related:

- Ethical AI
- Residual Ethical Risk
- Ethical Trade-offs

---

# Ethical Reasoning

When evaluating an ethical claim about AI, ask:

1. What is the system intended to achieve?
2. Should AI be used for this task?
3. What values are involved?
4. Which rights may be affected?
5. Who benefits?
6. Who may be harmed?
7. Who has decision-making power?
8. What assumptions are being made?
9. What evidence supports the claim?
10. What evidence would falsify or materially weaken it?
11. What causal mechanisms may explain the observed outcome?
12. What alternative explanation exists?
13. Which ethical theories or principles support or challenge the conclusion?
14. What reasonable counterargument exists?
15. What uncertainty remains?
16. What alternatives to the proposed AI system exist?
17. What residual risk remains after controls?
18. Who has legitimate authority to accept that remaining risk?
19. What evidence would justify restriction, suspension, redesign, or retirement?

Related:

→ 017 MOC - Ethical Trade-offs & Decision Reasoning

---

# Foundational Reasoning Pattern

A useful high-level reasoning pattern is:

**Purpose & Alternatives**

↓

**Stakeholders & Power**

↓

**Values & Rights**

↓

**Potential Harms & Risks**

↓

**Empirical & Causal Evidence**

↓

**Ethical Principles**

↓

**Requirements**

↓

**Controls & Assurance Evidence**

↓

**Residual Risk**

↓

**Governance Decision**

↓

**Monitoring & Reassessment**

This pattern is iterative rather than strictly linear.

New evidence, stakeholder input, incidents, or contextual changes may require earlier assumptions and decisions to be revisited.

---

# Related Domains

- 007 MOC - Human Rights Justice & Inclusion
- 008 MOC - Harm Risk & Power
- 009 MOC - Bias & Fairness
- 010 MOC - Privacy & Data Governance
- 011 MOC - Transparency Interpretability & Explainability
- 012 MOC - Human Agency Autonomy & Oversight
- 013 MOC - Safety Security Robustness & Reliability
- 014 MOC - Accountability Contestability & Redress
- 017 MOC - Ethical Trade-offs & Decision Reasoning
- 018 MOC - Governance Regulation & Legitimacy
- 019 MOC - Responsible AI Engineering & Assurance
- 020 MOC - Lifecycle Monitoring & Incident Management

---

# Open Questions

- Is there a universal ethical minimum for AI systems?
- Which ethical principles should take priority when they conflict?
- Who has legitimate authority to define acceptable AI use?
- Can ethical requirements be meaningfully operationalized without oversimplifying them?
- When should an ethical principle be treated as a constraint rather than an optimization objective?
- Should AI systems ever be regarded as moral agents?
- How should responsibility be distributed across complex AI supply chains?
- Can a legally compliant AI system nevertheless lack ethical legitimacy?
- How should uncertainty affect ethical judgments in high-risk applications?
- When should ethical analysis conclude that an AI system should not be deployed at all?
- What residual ethical risks, if any, may legitimately be accepted?
- What evidence should trigger restriction, suspension, redesign, or retirement?

---

## Continue Exploring

→ 007 MOC - Human Rights Justice & Inclusion

→ 008 MOC - Harm Risk & Power

→ 017 MOC - Ethical Trade-offs & Decision Reasoning

→ 019 MOC - Responsible AI Engineering & Assurance
