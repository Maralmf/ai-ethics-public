---
type: moc
status: mature
domains:
  - harm-risk-power
created: 2026-09-01
updated: 2026-09-25
---

# Harm, Risk & Power

## Scope

This MOC organizes concepts concerning harm, risk, vulnerability, uncertainty, exposure, and power in the ethical evaluation of AI systems.

It examines not only whether an AI system can produce adverse outcomes, but:

- what kinds of harm may occur
- who may experience those harms
- how severe or reversible they may be
- how uncertainty affects risk judgments
- how harms and benefits are distributed
- who has the power to define, impose, avoid, challenge, or accept risk
- how harms may accumulate or propagate through socio-technical systems

The central questions are:

> **What can go wrong, who may be harmed, and through what mechanism?**

and:

> **Who has the power to create, impose, avoid, mitigate, contest, or accept the resulting risks?**

---

## Why This Domain Matters

AI systems can create benefits while simultaneously imposing burdens on different people or groups.

A system may:

- improve average performance while harming a minority
- reduce one type of risk while increasing another
- transfer risk from an organization to affected individuals
- create harms that are difficult to observe or quantify
- amplify pre-existing vulnerabilities
- produce cumulative effects through repeated decisions
- change institutional incentives and behavior
- create new dependencies or asymmetries of power

Therefore:

> **Aggregate system performance is not sufficient for ethical risk assessment.**

Ethical evaluation must examine the distribution, severity, reversibility, uncertainty, and governance of potential harms.

---

# Conceptual Orientation

A useful working relationship is:

**Context & Purpose**

↓

**Stakeholders**

↓

**Hazards / Sources of Harm**

↓

**Exposure**

↓

**Vulnerability**

↓

**Potential Harm**

↓

**Likelihood & Severity**

↓

**Risk**

↓

**Distribution of Risk**

↓

**Controls**

↓

**Residual Risk**

↓

**Governance Decision**

↓

**Monitoring & Reassessment**

Power affects every stage of this chain.

It influences:

- who defines the purpose
- which harms are considered relevant
- whose evidence counts
- which risks are tolerated
- who can refuse exposure
- who can demand mitigation
- who can contest the decision
- who is authorized to accept residual risk

This is a conceptual orientation rather than a universal formal risk model.

---

# Harm

- Harm

Harm refers broadly to adverse effects on persons, groups, communities, institutions, society, or other ethically relevant entities.

Potential harms may affect:

- wellbeing
- rights
- opportunities
- resources
- autonomy
- reputation
- security
- social participation
- dignity
- access to essential services

Harm should not be reduced to physical injury.

---

## Individual Harm

- Individual Harm

Individual harms affect identifiable persons.

Examples may include:

- denial of employment
- denial of credit
- incorrect medical recommendation
- reputational damage
- privacy loss
- financial loss
- psychological distress
- unjustified surveillance
- loss of autonomy

### Key Question

> What happens to the individual when the system is wrong, misused, or applied inappropriately?

---

## Group Harm

- Group Harm

Group harms affect people partly because of their membership, perceived membership, or position within a socially relevant group.

Examples may include:

- systematic exclusion
- discriminatory error patterns
- stigmatization
- stereotyping
- unequal allocation of resources
- differential exposure to surveillance

Group harms cannot always be understood simply by summing individual harms.

Related:

- Representational Harm
- Allocative Harm
- 009 MOC - Bias & Fairness

---

## Societal Harm

- Societal Harm

Some AI-related harms may emerge at institutional or societal scale.

Examples may include:

- erosion of trust
- normalization of surveillance
- concentration of power
- degradation of information environments
- labor displacement
- institutional dependency
- weakening of democratic participation
- systemic discrimination

### Core Insight

A system may create relatively small individual effects while still producing substantial cumulative societal consequences.

---

# Types of Harm

A useful harm taxonomy may include:

## Physical Harm

- Physical Harm

Injury, illness, unsafe conditions, or threats to bodily integrity.

---

## Psychological Harm

- Psychological Harm

Distress, anxiety, humiliation, coercion, manipulation, or reduced sense of agency.

---

## Economic Harm

- Economic Harm

Loss of income, employment, credit, insurance, property, or economic opportunity.

---

## Reputational Harm

- Reputational Harm

Damage to social standing, credibility, professional reputation, or perceived trustworthiness.

---

## Informational Harm

- Informational Harm

Harms associated with inappropriate collection, inference, disclosure, manipulation, or use of information.

Related:

→ 010 MOC - Privacy & Data Governance

---

## Allocative Harm

- Allocative Harm

Occurs when systems affect access to resources, services, opportunities, or benefits.

Examples:

- hiring
- lending
- healthcare allocation
- insurance
- education admissions

---

## Representational Harm

- Representational Harm

Occurs when systems reinforce degrading, stereotypical, exclusionary, or distorted representations of people or groups.

Representational harms may exist even when no immediate resource allocation occurs.

---

## Autonomy Harm

- Autonomy Harm

Occurs when AI systems improperly influence, constrain, substitute for, or undermine meaningful human choice.

Related:

→ 012 MOC - Human Agency Autonomy & Oversight

---

# Direct and Indirect Harm

## Direct Harm

- Direct Harm

The AI-enabled process contributes relatively immediately to an adverse outcome.

Example:

> An unsafe autonomous system causes physical injury.

---

## Indirect Harm

- Indirect Harm

Harm arises through downstream institutional, behavioral, or social mechanisms.

Example:

> Automated ranking changes organizational behavior in ways that systematically reduce opportunities for a group.

### Core Insight

The absence of direct causation does not imply the absence of ethical responsibility.

---

# Cumulative and Compounding Harm

- Cumulative Harm
- Compounding Harm

Repeated small disadvantages may accumulate into significant long-term harm.

For example:

**slightly lower ranking**

↓

**fewer opportunities**

↓

**less experience**

↓

**weaker future profile**

↓

**future ranking disadvantage**

This may produce feedback loops.

Related:

- Feedback Loop
- Historical Bias
- Structural Inequality

---

# Risk

- Risk

Risk concerns the possibility of adverse outcomes under conditions of uncertainty.

A common simplified representation is:

\[
Risk \approx Likelihood \times Severity
\]

This formulation can be useful as a heuristic, but it should not be treated as a complete ethical definition of risk.

Ethically relevant risk assessment may also require consideration of:

- uncertainty
- exposure
- vulnerability
- reversibility
- detectability
- duration
- affected population
- distribution
- systemic effects
- ability to contest or recover
- availability of alternatives

---

# Hazard, Harm, and Risk

These concepts should remain distinct.

### Hazard

- Hazard

A source or condition with the potential to cause harm.

### Harm

- Harm

The adverse consequence itself.

### Risk

- Risk

The possibility and significance of harm occurring under particular conditions.

A useful distinction is:

**Hazard**

→ what could cause harm?

**Exposure**

→ who encounters the hazard?

**Vulnerability**

→ how susceptible are they to harm?

**Harm**

→ what adverse consequence may result?

**Risk**

→ how should the possibility and significance of that harm be evaluated?

---

# Likelihood

- Likelihood

Likelihood concerns how plausible or probable a harmful outcome is.

However:

> **Low probability does not automatically imply low ethical importance.**

A low-probability event may deserve substantial attention when:

- harm would be catastrophic
- effects are irreversible
- vulnerable populations are exposed
- uncertainty is high
- recovery is difficult

---

# Severity

- Severity

Severity concerns the magnitude or seriousness of potential harm.

Relevant dimensions may include:

- intensity
- duration
- reversibility
- number of people affected
- rights affected
- downstream consequences

---

# Exposure

- Exposure

Exposure concerns whether, how often, and under what conditions people or systems encounter a source of harm.

Two groups facing the same technical hazard may experience different risk because their exposure differs.

---

# Vulnerability

- Vulnerability

Vulnerability concerns increased susceptibility to harm or reduced capacity to avoid, contest, recover from, or adapt to adverse effects.

Vulnerability should not be treated only as an inherent characteristic of individuals.

It may arise from:

- dependency
- poverty
- disability
- institutional position
- lack of bargaining power
- digital exclusion
- legal status
- informational disadvantage
- absence of meaningful alternatives

Therefore:

> **Vulnerability is often relational and context-dependent.**

Related:

→ 007 MOC - Human Rights Justice & Inclusion

---

# Uncertainty

- Uncertainty

Ethical risk assessment must distinguish uncertainty from known risk.

Relevant sources may include:

- insufficient data
- model uncertainty
- measurement uncertainty
- causal uncertainty
- distribution shift
- unknown deployment conditions
- unforeseen user behavior
- emerging social effects

### Key Question

> What do we not know, and how should that uncertainty affect the decision?

A precise risk estimate should not create false confidence when the underlying evidence is weak.

---

---

# Risk Is Not Only an Expected Value

A system may appear favorable under an average expected-loss calculation while remaining ethically problematic.

For example:

```text
Expected average benefit = high

but

a small group faces severe or irreversible harm
```

An expected-value calculation can obscure ethically relevant features such as:

- concentrated harm
- catastrophic outcomes
- irreversible consequences
- rights violations
- unequal exposure
- vulnerability
- uncertainty
- lack of meaningful consent
- inability to contest or recover
- distribution of benefits and burdens

Therefore:

> **Expected value is one analytical input, not a complete ethical decision rule.**

A risk may remain ethically unacceptable even when its average expected cost appears low.

---

# Reversibility & Recoverability

- Reversibility
- Recoverability

### Reversibility

asks:

> Can the effects of a decision realistically be undone?

### Recoverability

asks:

> If harm occurs, can affected people, institutions, or systems return to an acceptable state?

Some AI-mediated harms may be difficult or impossible to reverse.

Examples may include:

- irreversible disclosure of sensitive information
- wrongful deprivation of an opportunity that cannot later be restored
- persistent reputational damage
- physical injury
- long-term exclusion
- institutionalization of harmful decision practices
- widespread release of unsafe capabilities

### Core Principle

> **The less reversible a potential harm is, the stronger the case may be for prevention, precaution, stronger evidence, and earlier intervention.**

---

# Detectability & Latency

- Detectability
- Harm Latency

Some harms are visible immediately.

Others may emerge only after:

- repeated decisions
- long-term deployment
- interaction with institutional incentives
- cumulative disadvantage
- changes in user behavior
- feedback loops
- expansion to new populations or contexts

A harm that is difficult to detect may remain unaddressed for long periods.

Therefore risk analysis should ask:

- How quickly would harm become visible?
- Who would be able to detect it?
- What evidence would reveal it?
- Could the affected people report it?
- Are monitoring systems capable of identifying it?
- Would the organization have incentives to notice it?

### Core Principle

> **Low detectability can increase ethical significance even when estimated likelihood is unchanged.**

---

# Systemic Risk

- Systemic Risk

Some AI-related risks are not confined to a single model decision or user.

They may propagate through:

- institutions
- markets
- infrastructures
- information ecosystems
- public services
- supply chains
- interconnected automated systems

Potential systemic effects may include:

- correlated failures
- widespread dependency on the same model or provider
- concentration of decision-making power
- shared vulnerabilities
- common-mode errors
- cascading operational failures
- ecosystem-wide misinformation
- normalization of harmful institutional practices

### Key Question

> Could failure or misuse in one component propagate beyond the immediate system or decision?

### Important

Systemic risk should not be inferred merely because a system is large.

Relevant questions include:

- interdependence
- substitutability
- concentration
- propagation pathways
- correlated exposure
- recovery capacity

---

# Risk Distribution

Risk is not ethically neutral simply because total expected harm is low.

A central question is:

> **Who receives the benefits, and who bears the risks?**

A system may:

- concentrate benefits among institutions while externalizing harm to individuals
- distribute small benefits widely while imposing severe burdens on a minority
- protect powerful actors while increasing exposure for less powerful groups
- reduce organizational costs while shifting error costs to affected communities

A useful distinction is:

**Aggregate Risk**

→ how much risk exists overall?

versus:

**Distributed Risk**

→ who bears which risks, under what conditions, and with what capacity to refuse or recover?

Related:

- Distributive Justice
- 007 MOC - Human Rights Justice & Inclusion

---

# Risk Transfer & Externalization

- Risk Transfer
- Risk Externalization

Organizations may reduce their own exposure while transferring risk to others.

Examples include:

- automating a decision to reduce organizational cost while increasing contestability burdens on individuals
- using automated fraud detection that reduces financial loss but increases wrongful account restrictions
- shifting monitoring labor to users
- deploying systems whose environmental or social costs are borne elsewhere

### Key Question

> Does the system reduce risk, or merely move it to actors with less power?

### Core Principle

> **Risk reduction for one stakeholder should not automatically be treated as overall risk reduction.**

---

# Power

Power is not an additional variable at the end of risk analysis.

It can shape the entire process.

Relevant forms may include:

- institutional power
- economic power
- informational power
- technical expertise
- agenda-setting power
- decision-making authority
- control over infrastructure
- ability to define acceptable evidence
- ability to impose or refuse risk

### Key Question

> Who can define the problem, choose the system, set the thresholds, accept the risk, and stop the deployment?

Power affects:

- whose harms are recognized
- whose evidence is considered credible
- which trade-offs are accepted
- who must provide justification
- who can refuse participation
- who can demand mitigation
- who can challenge outcomes
- who receives remedy

---

# Power Asymmetry

- Power Asymmetry

Power asymmetry exists when stakeholders differ substantially in their capacity to:

- make decisions
- shape system design
- impose conditions
- access resources
- obtain information
- refuse participation
- challenge decisions
- demand correction
- influence governance

Examples may include relationships between:

- employer and employee
- platform and user
- lender and borrower
- government agency and citizen
- insurer and applicant
- healthcare institution and patient

### Core Insight

> **The same technical risk may have different ethical significance depending on who has the power to avoid, contest, or recover from it.**

---

# Information Asymmetry

- Information Asymmetry

Information asymmetry arises when one party possesses substantially more relevant information than another.

In AI-mediated decisions, an organization may know:

- that AI is being used
- which data were used
- how the system was evaluated
- what its limitations are
- which thresholds were selected
- what uncertainty exists
- how decisions can be overridden

while the affected individual may know little or none of this.

Information asymmetry can affect:

- informed choice
- consent
- contestability
- bargaining power
- ability to identify errors
- ability to seek redress

Related:

- Transparency
- Contestability
- 014 MOC - Accountability Contestability & Redress

---

# Dependency & Lack of Alternatives

- Dependency
- Meaningful Choice

Exposure to risk is ethically different when people have realistic alternatives.

A person may formally be able to refuse an AI-mediated process while, in practice, refusal means losing access to:

- employment
- credit
- healthcare
- education
- essential public services
- communication infrastructure
- social participation

Therefore:

> **Formal choice ≠ Meaningful choice**

Risk evaluation should consider whether affected stakeholders can realistically:

- opt out
- choose an alternative
- obtain human review
- seek another provider
- avoid repeated exposure
- challenge the process without retaliation or excessive burden

---

# Risk Assessment

- Risk Assessment

Risk assessment is the structured process of identifying and evaluating potential adverse outcomes.

A robust assessment may consider:

1. **Purpose & Context**
2. **Stakeholders**
3. **Hazards / Sources of Harm**
4. **Exposure**
5. **Vulnerability**
6. **Potential Harms**
7. **Likelihood**
8. **Severity**
9. **Uncertainty**
10. **Distribution**
11. **Reversibility**
12. **Detectability**
13. **Power & Dependency**
14. **Existing Controls**
15. **Residual Risk**
16. **Available Alternatives**

### Important

Risk assessment is not identical to risk acceptance.

Assessment can provide evidence concerning:

- what may happen
- how serious it may be
- who may be affected
- how uncertain the evidence is
- whether controls appear effective

But it does not by itself answer:

> **Should the remaining risk be accepted?**

---

# Risk Estimation vs Risk Acceptability

This distinction is central.

### Risk Estimation

asks:

> What risk appears to exist, given the available evidence and assumptions?

### Risk Acceptability

asks:

> Is that risk ethically, legally, and institutionally acceptable under the circumstances?

Risk acceptability may depend on:

- affected rights
- severity of harm
- distribution of risk
- vulnerability
- reversibility
- uncertainty
- necessity
- proportionality
- available alternatives
- stakeholder participation
- legitimacy of decision authority
- effectiveness of controls
- monitoring capacity

Therefore:

> **Risk estimation ≠ Risk acceptability**

A technically precise estimate cannot determine by itself whether imposing that risk is ethically justified.

---

# Controls

- Technical Control
- Organizational Control
- Governance Control

Controls are interventions intended to prevent, reduce, detect, contain, or respond to risk.

### Technical Controls

may include:

- input validation
- access control
- robustness measures
- uncertainty estimation
- threshold design
- monitoring
- fail-safe behavior

### Organizational Controls

may include:

- review procedures
- staff training
- role separation
- escalation pathways
- approval processes
- incident response
- human oversight

### Governance Controls

may include:

- deployment restrictions
- independent review
- audit requirements
- documentation obligations
- contestability
- redress
- stop authority

### Core Principle

> **A control should be linked to a specific risk mechanism and supported by evidence of effectiveness.**

---

# Residual Risk

- Residual Risk
- Residual Ethical Risk

Residual risk is the risk that remains after relevant controls have been applied.

A system may still retain:

- uncertain failure modes
- unresolved subgroup harms
- privacy exposure
- misuse potential
- monitoring gaps
- safety limitations
- institutional dependencies
- irreversible consequences

Residual risk should therefore be explicitly documented rather than implicitly ignored.

### Key Questions

- What remains after mitigation?
- Who bears that remaining risk?
- How uncertain is the estimate?
- What evidence supports the claim that controls are effective?
- Is the residual risk reversible?
- What monitoring is required?
- Who has authority to accept it?

---

# Risk Acceptance & Authority

- Risk Acceptance
- Risk Owner
- Legitimate Authority

A governance process may decide to:

- accept risk
- reduce risk further
- restrict deployment
- change deployment conditions
- redesign the system
- suspend use
- choose a non-AI alternative
- reject deployment

But a central ethical question remains:

> **Who has legitimate authority to accept residual risk, especially when others bear the consequences?**

The organization deploying a system should not automatically be assumed to possess legitimate authority to impose risk on affected populations merely because it owns or operates the system.

Relevant considerations may include:

- legal authority
- institutional mandate
- stakeholder participation
- rights constraints
- distribution of benefits and burdens
- conflicts of interest
- accountability
- contestability
- availability of redress

---

# Precaution, Proportionality & Necessity

Risk reasoning may require more than expected harm estimates.

Relevant concepts include:

- Precaution
- Proportionality
- Necessity
- Reversibility
- Burden of Proof

### Necessity

asks whether the objective requires the proposed AI intervention or whether a less intrusive or less risky alternative could achieve the goal.

### Proportionality

asks whether the expected benefits justify the severity, distribution, likelihood, and nature of the risks imposed.

### Precaution

may become especially relevant when:

- potential harm is severe
- uncertainty is substantial
- consequences may be irreversible
- affected groups are highly vulnerable
- evidence is incomplete

### Core Principle

> **Greater potential harm, uncertainty, and irreversibility can justify stronger evidence requirements, safeguards, and limits on deployment.**

Related:

→ 017 MOC - Ethical Trade-offs & Decision Reasoning

---

# Monitoring & Risk Drift

Risk is not necessarily static.

After deployment, changes may occur in:

- data
- populations
- model behavior
- institutional practices
- user behavior
- deployment scope
- external threats
- subgroup outcomes
- power relationships
- available alternatives

A system that was acceptable under one set of conditions may become unacceptable under another.

Related:

- Post-Deployment Monitoring
- Data Drift
- Concept Drift
- Fairness Drift
- 020 MOC - Lifecycle Monitoring & Incident Management

### Core Principle

> **Initial risk assessment ≠ Permanent risk acceptability**

---

# Relationship to Human Rights & Justice

→ 007 MOC - Human Rights Justice & Inclusion

Harm and risk analysis becomes ethically richer when connected to:

- rights
- dignity
- justice
- equality
- non-discrimination
- vulnerability
- participation

A risk may be ethically significant not only because of its expected magnitude but because:

- a fundamental right is affected
- burdens fall on already disadvantaged groups
- the affected person did not meaningfully consent
- the exposure is unavoidable
- remedy is unavailable

---

# Relationship to Bias & Fairness

→ 009 MOC - Bias & Fairness

Bias and fairness analysis can identify patterns of disparity.

Harm and risk analysis asks additional questions:

- What consequences follow from the disparity?
- How severe are they?
- Who is exposed?
- Are harms reversible?
- What uncertainty remains?
- Do feedback loops compound the effect?
- What controls are available?

Therefore:

> **A statistical disparity is evidence to interpret, not a complete characterization of harm.**

---

# Relationship to Safety, Security & Reliability

→ 013 MOC - Safety Security Robustness & Reliability

Safety and security mechanisms can reduce certain harms and risks.

However:

- a safe system can still be unjust
- a secure system can still violate rights
- a reliable system can still be used for an illegitimate purpose

Therefore technical safety evidence is necessary in some contexts but not sufficient for overall ethical acceptability.

---

# Relationship to Accountability & Redress

→ 014 MOC - Accountability Contestability & Redress

Risk governance requires clear answers to:

- Who owns the risk?
- Who monitors it?
- Who receives incident reports?
- Who can escalate?
- Who can stop the system?
- Who answers for harmful outcomes?
- How can affected people contest a decision?
- What remedy is available?

A risk-control system without accountability may fail even when technical monitoring exists.

---

# Relationship to Governance

→ 018 MOC - Governance Regulation & Legitimacy

Governance determines:

- who has decision authority
- what evidence is required
- which risks are tolerable
- which constraints are mandatory
- who can approve deployment
- who can impose conditions
- who can suspend or stop the system

Risk governance therefore involves both empirical assessment and normative or institutional judgment.

---

# Practical Evaluation Lens

When evaluating an AI-enabled system, ask:

## Purpose & Alternatives

- What is the system intended to achieve?
- Should AI be used for this task?
- Is there a less harmful or less risky alternative?

## Harm

- What adverse outcomes are plausible?
- Are harms individual, group-level, institutional, or societal?
- Could harms accumulate over time?

## Hazard & Mechanism

- What could cause each harm?
- Through what technical, organizational, or social mechanism?

## Exposure

- Who encounters the hazard?
- How often?
- Can exposure be avoided?

## Vulnerability

- Who is especially susceptible?
- Who has limited ability to refuse, contest, or recover?

## Likelihood

- How plausible is the harm?
- How strong is the evidence?

## Severity

- How serious could the harm be?
- How many people may be affected?
- Are rights implicated?

## Reversibility

- Can the harm realistically be undone?
- Can affected people recover?

## Distribution

- Who receives the benefits?
- Who bears the risks?

## Power

- Who defines the acceptable risk?
- Who can refuse?
- Who can demand mitigation?
- Who can stop the system?

## Uncertainty

- What is unknown?
- Could the estimate create false confidence?

## Controls

- What prevents or reduces the harm?
- What evidence shows that the controls work?

## Residual Risk

- What remains after controls?
- Who bears it?

## Governance

- Who has legitimate authority to accept or reject the residual risk?

## Monitoring

- What evidence would show that risk has changed?
- What should trigger investigation, restriction, suspension, redesign, or retirement?

---

# Example — AI-Assisted Credit Decision

Consider an AI system used to support consumer credit decisions.

A narrow analysis might ask:

> Is the model accurate?

A harm, risk, and power analysis asks additional questions.

### Harm

Could an incorrect denial prevent access to housing, education, or emergency resources?

### Exposure

Which applicants are most frequently subject to the system?

### Vulnerability

Which applicants have the fewest alternative sources of credit or the least ability to absorb an error?

### Distribution

Does the institution receive efficiency benefits while applicants bear most error costs?

### Information Asymmetry

Does the lender know substantially more about the model, data, and decision process than the applicant?

### Power

Can an applicant meaningfully refuse automated assessment?

### Contestability

Can an applicant identify and challenge incorrect data or an erroneous decision?

### Reversibility

Can a wrongful denial be corrected before the lost opportunity becomes irreversible?

### Residual Risk

What harmful errors remain after mitigation?

### Governance

Who has authority to accept those remaining risks, and on what basis?

This illustrates why:

> **Model performance is evidence about one part of the system, not a complete ethical risk assessment.**

---

# Common Failure Modes in Risk Reasoning

### "Low probability means low ethical importance."

Not necessarily.

Severity, irreversibility, vulnerability, and uncertainty also matter.

---

### "High average benefit justifies concentrated harm."

Not automatically.

Distribution and rights require separate evaluation.

---

### "If a risk can be quantified, the ethical decision is objective."

False.

Quantification can inform judgment but does not determine risk acceptability.

---

### "Risk is only a technical property of the model."

False.

Risk can arise from data, institutions, deployment, incentives, human behavior, and power relations.

---

### "Mitigation eliminates risk."

Not necessarily.

Residual risk should be identified and governed explicitly.

---

### "If users can opt out, exposure is voluntary."

Not necessarily.

Formal opt-out may not constitute meaningful choice when alternatives are unavailable or costly.

---

### "The organization deploying the system can decide which risks are acceptable."

Not automatically.

Legitimate risk-acceptance authority depends on rights, law, institutional mandate, accountability, and who bears the consequences.

---

### "Monitoring solves post-deployment risk."

False.

Monitoring is useful only when signals are linked to responsibility, decision authority, and intervention mechanisms.

---

# Evidence & Normative Status

Claims in this domain may have different status.

Distinguish among:

- **empirical claims** — what outcomes, disparities, incidents, exposures, or failures are observed
- **causal claims** — what mechanisms are proposed to produce those outcomes
- **risk estimates** — judgments or models concerning likelihood, severity, exposure, and uncertainty
- **normative claims** — what risks ought to be prevented, reduced, tolerated, or rejected
- **governance decisions** — what an authorized institution decides under specified evidence, constraints, and responsibilities

These categories are related but not interchangeable.

For example:

**Estimated risk = low**

does not automatically establish:

**risk is ethically acceptable**

and:

**risk is ethically concerning**

does not automatically establish:

**a particular causal mechanism has been proven**

Therefore:

> **Evidence can estimate and characterize risk; it does not by itself determine whether imposing that risk is justified.**

---

# Ethical Reasoning Chain

A useful reasoning sequence is:

**Purpose & Alternatives**

↓

**Stakeholders & Power**

↓

**Hazards / Sources of Harm**

↓

**Exposure & Vulnerability**

↓

**Potential Harms**

↓

**Likelihood, Severity & Uncertainty**

↓

**Distribution & Reversibility**

↓

**Controls**

↓

**Assurance Evidence**

↓

**Residual Risk**

↓

**Risk-Acceptance Authority**

↓

**Governance Decision**

↓

**Deployment Conditions**

↓

**Monitoring**

↓

**Trigger / Incident**

↓

**Reassessment / Restrict / Redesign / Suspend / Retire**

This sequence is iterative rather than strictly linear.

New evidence may require earlier assumptions, controls, or governance decisions to be revisited.

---

# Related MOCs

### Foundations
→ 006 MOC - Foundations & Ethical Theory

### Human Rights & Justice
→ 007 MOC - Human Rights Justice & Inclusion

### Bias & Fairness
→ 009 MOC - Bias & Fairness

### Privacy & Data Governance
→ 010 MOC - Privacy & Data Governance

### Human Agency
→ 012 MOC - Human Agency Autonomy & Oversight

### Safety, Security & Reliability
→ 013 MOC - Safety Security Robustness & Reliability

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

## Risk & Safety

- risk assessment and risk-management literature
- safety engineering
- human factors
- resilience and systems safety
- uncertainty and decision-making under risk

## Harm & Social Impact

- algorithmic harm
- allocative and representational harm
- cumulative disadvantage
- sociotechnical systems research
- institutional and structural analysis

## Power & Vulnerability

- power asymmetry
- dependency
- vulnerability
- information asymmetry
- critical data and technology studies

## Governance

- risk governance
- impact assessment
- assurance
- accountability
- incident management
- precaution and proportionality

Specific sources should be maintained as dedicated literature, framework, or evidence notes and linked to the relevant concepts.

---

# Open Questions

- Which AI-related harms are systematically under-measured because they are difficult to quantify?
- How should low-probability, high-severity harms be compared with frequent lower-severity harms?
- When should rights-based constraints override expected-value calculations?
- How should uncertainty affect the burden of proof for deployment?
- Who has legitimate authority to accept residual risk on behalf of affected populations?
- How should risk analysis account for people who cannot meaningfully opt out?
- When does risk transfer become ethically unjustifiable externalization?
- How should cumulative and compounding harms be measured over long time horizons?
- When does an AI risk become systemic rather than local?
- How should risk assessment incorporate changing power relationships after deployment?
- What evidence is sufficient to conclude that a control meaningfully reduces harm?
- When should residual risk require restricted deployment or non-deployment?
- How should precaution be applied without treating all uncertainty as a reason for prohibition?
- What monitoring evidence should trigger investigation, restriction, suspension, redesign, or retirement?

---

## Continue Exploring

→ 009 MOC - Bias & Fairness

→ 012 MOC - Human Agency Autonomy & Oversight

→ 013 MOC - Safety Security Robustness & Reliability

→ 014 MOC - Accountability Contestability & Redress

→ 017 MOC - Ethical Trade-offs & Decision Reasoning

→ 020 MOC - Lifecycle Monitoring & Incident Management
