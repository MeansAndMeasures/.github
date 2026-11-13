# Accessibility

**Means+Measures**

**Equity of means. Equality of measures.**

Accessibility is a condition of meaningful participation. A system is not adequately accessible merely because its information or functionality technically exists. People must be able to understand, navigate, and use it through means appropriate to their circumstances.

Means+Measures treats accessibility as part of system functionality, institutional responsibility, and accountable design.

## 1. Purpose and scope

This document establishes accessibility expectations for Means+Measures repositories, documentation, interfaces, development practices, and contribution processes.

Individual projects may establish additional requirements appropriate to their users, technologies, functions, and applicable obligations.

This document does not assert that every Means+Measures project presently conforms to a particular accessibility standard or certification.

## 2. Accessibility as a design responsibility

**Lack of privilege is not lack of access.**

Access should not depend unnecessarily on specialized equipment, professional assistance, institutional affiliation, particular communication methods, or familiarity with technical systems.

Accessibility considerations belong within the design and implementation process rather than being postponed until after a system has been completed.

Responsibility includes examining how people interact with a system in practice, not simply whether its components satisfy a checklist.

An accessible system should support meaningful use of its intended functions, including the ability to recognize errors, recover from them, and understand consequential decisions.

## 3. Areas of consideration

Accessibility evaluation may include:

### Perception and presentation

- Text readability, contrast, scaling, and legibility.
- Screen-reader compatibility and semantic structure.
- Alternatives for meaningful visual and auditory information.
- Information conveyed through more than color alone.
- Layouts that remain understandable across devices and display configurations.

### Interaction and navigation

- Keyboard access and predictable navigation.
- Appropriate focus management and visible interaction states.
- Compatibility with assistive technologies.
- Alternatives to unnecessarily precise gestures or time-sensitive interactions.
- Forms with understandable labels, instructions, validation, and error recovery.

### Comprehension and communication

- Clear terminology and explanations.
- Understandable navigation and task progression.
- Consistent presentation of requirements and decisions.
- Support for different communication methods where practical.
- Avoidance of unnecessary procedural complexity or demands for specialized knowledge.

### Institutional and procedural access

Accessibility also concerns processes through which people obtain information, request assistance, challenge decisions, or exercise available rights.

A technically accessible interface does not necessarily establish an accessible process if successful participation still depends on avoidable institutional or procedural barriers.

## 4. Standards and evaluation

Relevant accessibility standards and guidance may inform project requirements and evaluation, including:

- Web Content Accessibility Guidelines (WCAG).
- Web Accessibility Initiative Accessible Rich Internet Applications (WAI-ARIA).
- Platform-specific accessibility guidance.
- Applicable legal or contractual accessibility obligations.
- Direct testing and feedback from people using the system.

The appropriate standard, version, conformance target, and testing methodology should be identified at the project level where necessary.

Automated testing may reveal detectable defects, but a passing automated test does not establish complete accessibility.

Evaluation should also consider manual testing, realistic task completion, assistive-technology interactions, and observed barriers.

Conformance claims must be supported by evidence appropriate to their scope.

## 5. Accessibility in development and review

Accessibility should be considered throughout a project's development lifecycle.

### Requirements and design

Identify the people and tasks the system is intended to support, the conditions of use, and barriers that could materially affect participation.

Distinguish established requirements from proposed implementation choices.

### Implementation

Use appropriate semantic structures, interaction patterns, and platform capabilities.

Avoid introducing dependencies or restrictions that unnecessarily exclude otherwise legitimate users.

### Validation

Test relevant functionality using methods proportionate to the component and its intended use.

Record what was tested, what was observed, and what remains unverified.

### Review

Review proposed changes for their effects on accessibility, including whether previously available means of interaction remain functional.

A change that improves one aspect of accessibility may create a different barrier. Such tradeoffs should be evaluated rather than assumed away.

### Maintenance

Accessibility is subject to regression as software, dependencies, content, and user needs change.

Identified barriers should be documented and reassessed as appropriate.

## 6. Reporting an accessibility barrier

Accessibility concerns may be reported through the affected repository's **Issues** tab using the **Accessibility barrier** template.

A useful report identifies:

- The barrier encountered.
- The intended task or outcome.
- The affected feature, process, or documentation.
- Relevant conditions of use, if known.
- The effect on access or participation.
- Supporting observations or evidence, when available.

Reporters are not required to disclose a disability, diagnosis, medical history, or assistive-technology use merely to establish that a barrier exists.

A report does not require a complete technical solution, a cited WCAG criterion, or a reproducible test case.

### Confidential accessibility concerns

For reports involving sensitive personal information or individual circumstances, contact:

**privacy-contact@mail.meansandmeasures.com**

This mailbox supports OpenPGP encryption.

Public key: [`PGP_PUBLIC_KEY.asc`](PGP_PUBLIC_KEY.asc)

Fingerprint:

`B0BA F819 B84B E96E CF22 B60C AD9C CEA6 3C3F BB30`

Verify the public key's fingerprint before encrypting sensitive correspondence.

Encryption is optional. OpenPGP does not necessarily conceal email metadata.

## 7. Assessment and resolution

Accessibility reports should be evaluated according to the barrier identified, the relevant functionality, the affected people and tasks, and the available evidence.

Assessment should distinguish:

- **Observed barrier:** What prevents or complicates participation?
- **Functional consequence:** What task or outcome is affected?
- **Underlying cause:** What is known about the source of the barrier?
- **Corrective options:** What changes could address it?
- **Verification:** How can an improvement be meaningfully evaluated?

A report may lead to an implementation change, documentation improvement, alternative interaction method, further investigation, or another appropriate response.

Resolution should be assessed against the accessibility outcome, not solely whether an issue was closed or a change was merged.

Where a limitation remains unresolved, its existence, consequences, and available alternatives should be documented where practical.

## 8. Accessibility of participation itself

Means+Measures contribution and review processes are also subject to accessibility considerations.

Participants should be able to raise concerns, provide evidence, propose improvements, and question decisions without unnecessary reliance on specialized terminology or inaccessible procedures.

Where practical, project processes should accommodate different communication and interaction methods.

The inability to complete a particular form or use a particular interface should not automatically invalidate an otherwise legitimate concern.

Accessibility requests and contributions should be evaluated on their merits rather than the contributor's credentials, institutional standing, or ability to supply a technical implementation.

## 9. Accountability and continuous improvement

Accessibility is evaluated through demonstrated conditions of use and their effects on participation.

An institution's intentions, policies, or formal assurances do not substitute for evidence of accessible outcomes.

Means+Measures should apply to its own systems the standards of transparency, scrutiny, and accountability that it expects of the institutions whose systems it helps improve.

Relevant barriers, corrective decisions, and validation results should retain sufficient context for future review.

## Related policies

- [CONTRIBUTING.md](CONTRIBUTING.md): How to participate and propose changes.
- [SUPPORT.md](SUPPORT.md): Support channels and assistance.
- [GOVERNANCE.md](GOVERNANCE.md): Decision-making and accountability.
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md): Community conduct and confidential reporting.
- [SECURITY.md](SECURITY.md): Vulnerability reporting and security procedures.

## Governing principle

**Equity of means:** Lack of privilege is not lack of access.

**Equality of measures:** Impacts are judged on their own merits, not the standing of the institution.

Institutions bear responsibility down through systems for making participation accessible.

Authority rises up through people who question, evaluate, and hold those institutions accountable.