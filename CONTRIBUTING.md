# Contributing Guidelines

Thank you for your interest in contributing to the AI Ethics Knowledge Base.

This repository uses a controlled contribution model designed to preserve the integrity, security, and consistency of the public knowledge base.

Please read these guidelines before submitting any Pull Request.

---

## 1. Contribution Workflow

External contributors do not receive direct write access to the main repository.

All contributions must follow this workflow:

1. Fork the repository
2. Create a new branch in your fork
3. Make the proposed changes
4. Review your own changes
5. Submit a Pull Request to the `main` branch
6. Wait for maintainer review
7. Address any requested changes

No contribution becomes part of the official knowledge base until it has been reviewed and merged.

---

## 2. What You May Contribute

Contributions may include:

- new AI Ethics concept notes
- improvements to existing public notes
- corrections to factual or conceptual errors
- new public case studies
- links between related concepts
- literature notes based on legally accessible sources
- regulatory or governance updates
- improvements to terminology or taxonomy
- safe static images when clearly necessary

All contributions must be relevant to the scope of the repository.

---

## 3. Allowed File Types

Unless explicitly approved by the maintainer, contributions should be limited to:

- `.md`
- `.png`
- `.jpg`
- `.jpeg`
- `.webp`

Markdown is the preferred format.

---

## 4. Prohibited Files and Paths

Do not add or modify executable, configuration, automation, or environment files.

The following are not accepted through normal content contributions:

- `.obsidian/`
- `.github/workflows/`
- JavaScript files
- TypeScript files
- Python scripts
- shell scripts
- PowerShell scripts
- batch files
- executables
- binaries
- plugin files
- environment files
- credential files
- private keys
- certificates

Examples include:

- `.js`
- `.ts`
- `.py`
- `.sh`
- `.ps1`
- `.bat`
- `.exe`
- `.dll`
- `.jar`
- `.env`
- `.pem`
- `.key`
- `.p12`
- `.pfx`

Do not attempt to bypass these restrictions by changing file extensions or embedding executable payloads inside other files.

---

## 5. Sensitive Information

Never submit:

- passwords
- API keys
- authentication tokens
- session cookies
- private keys
- personal identifiers
- private research data
- confidential documents
- unpublished confidential manuscripts
- internal organizational information
- sensitive personal information

If sensitive information is accidentally included in a Pull Request, notify the maintainer immediately.

Do not assume that deleting the information in a later commit removes it from Git history.

---

## 6. Copyright and Source Material

Do not upload copyrighted papers, books, reports, datasets, figures, or other materials unless redistribution is legally permitted.

Prefer:

- DOI links
- official publication links
- citations
- your own summaries
- your own analytical notes

Do not upload full-text academic papers merely because you personally have access to them.

---

## 7. Note Design

Notes should preferably focus on one primary concept.

Use clear titles such as:

- `Algorithmic Bias.md`
- `Equalized Odds.md`
- `Human Oversight.md`
- `Fairness-Accuracy Trade-off.md`

Avoid vague filenames such as:

- `notes1.md`
- `new.md`
- `misc.md`
- `AI stuff.md`

---

## 8. Internal Linking

Use Obsidian-style internal links when connecting concepts:

`[[Algorithmic Bias]]`

`[[Human Oversight]]`

`[[EU AI Act]]`

Links should express meaningful conceptual relationships rather than being added only for quantity.

Where possible, explain the relationship in prose.

Preferred:

`[[Transparency]] can support [[Accountability]], but transparency alone does not guarantee [[Fairness]].`

Less useful:

`Related: [[Transparency]], [[Accountability]], [[Fairness]]`

---

## 9. Evidence and Sources

Factual claims should be supported by credible sources when appropriate.

Preferred sources include:

- peer-reviewed research
- official regulatory texts
- recognized standards bodies
- governmental publications
- established international organizations
- primary sources

Avoid presenting opinion, speculation, or unverified claims as established fact.

---

## 10. AI-Generated Content

AI tools may be used to assist drafting or editing, but contributors remain responsible for:

- factual accuracy
- source verification
- citation accuracy
- originality
- copyright compliance
- conceptual correctness

Unverified AI-generated material may be rejected.

---

## 11. Editing Existing Notes

Contributors may propose improvements to existing public notes.

However:

- do not delete substantial content without explaining why
- do not rename core taxonomy structures without justification
- do not remove citations without explanation
- do not rewrite large sections only for stylistic preference
- do not alter repository security or governance files unless specifically requested

Changes to repository governance files require explicit maintainer approval.

Examples include:

- `README.md`
- `CONTRIBUTING.md`
- `SECURITY.md`
- `.gitignore`
- `CODEOWNERS`
- branch or repository configuration

---

## 12. Pull Request Requirements

Each Pull Request should clearly explain:

### What changed?

Briefly describe the contribution.

### Why is this change useful?

Explain its relevance to the knowledge base.

### What type of contribution is it?

Examples:

- new concept
- correction
- literature note
- case study
- taxonomy improvement
- regulatory update

### Sources

List relevant sources when applicable.

### Security and privacy confirmation

By submitting the Pull Request, the contributor confirms that:

- no credentials or secrets are included
- no private or confidential information is included
- no prohibited executable files are included
- submitted content may be publicly visible

---

## 13. Pull Request Scope

Keep Pull Requests focused.

Preferred:

`Add note on Equalized Odds`

Avoid combining unrelated changes such as:

- adding several unrelated concepts
- restructuring the taxonomy
- changing security files
- modifying multiple unrelated cases

Small Pull Requests are easier to review and safer to merge.

---

## 14. Review and Approval

The maintainer may:

- request clarification
- request additional sources
- request formatting changes
- request smaller scope
- reject contributions
- edit accepted contributions before or after merging

Approval is based on:

- relevance
- accuracy
- clarity
- evidence quality
- consistency
- security
- maintainability

---

## 15. Security Model

All external contributions are treated as untrusted input until reviewed.

Contributors must not assume that access to the public repository provides access to:

- private notes
- private repositories
- the maintainer's Obsidian environment
- credentials
- unpublished material
- local files

The public repository is intentionally isolated from the private authoring environment.

---

## 16. Questions

If you are unsure whether a contribution is appropriate, discuss the proposed change before submitting a large Pull Request.

For security-sensitive matters, do not disclose sensitive details publicly.
