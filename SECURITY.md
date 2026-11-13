# Security Policy

**Means+Measures**

Security is a responsibility of system design, implementation, operation, and maintenance. It protects not only infrastructure and information, but also the ability of people to access and rely on the systems intended to serve them.

Means+Measures welcomes responsible vulnerability reports, security research, and contributions that improve the security and resilience of our projects.

## 1. Scope

This policy provides organization-wide guidance for reporting security vulnerabilities affecting Means+Measures repositories, software, and infrastructure.

Individual projects may maintain additional security documentation identifying supported versions, affected components, or project-specific reporting procedures.

The presence of a public repository does not imply that associated production systems, credentials, infrastructure, or third-party services are authorized targets for security testing.

## 2. Reporting a vulnerability

**Report security vulnerabilities privately. Do not disclose exploitable vulnerabilities through public issues, pull requests, or discussions.**

### Primary reporting path

Means+Measures provides a structured vulnerability reporting process through GitHub's private vulnerability reporting functionality.

For repositories where private vulnerability reporting is enabled:

1. Open the affected repository.
2. Navigate to **Security → Report a vulnerability**.
3. Complete the private vulnerability reporting form.
4. Submit the report for maintainer review.

The organization-wide reporting template is maintained at:

[`VULNERABILITY_REPORT.yml`](.github/VULNERABILITY_REPORT.yml)

Individual repositories may provide a project-specific reporting form when their requirements differ.

### Alternative reporting path: Private email

Security vulnerabilities, sensitive concerns, and matters involving repository maintainers or moderators may also be reported privately to:

**privacy-contact@mail.meansandmeasures.com**

This is the designated confidential contact for Means+Measures security and conduct-related concerns.

Reporters may use this address when GitHub's private vulnerability reporting functionality is unavailable or when email is the more appropriate reporting method.

### Encrypted reporting

The reporting mailbox supports OpenPGP encryption. Reporters may encrypt correspondence using the mailbox's public key.

**Public-key fingerprint (OpenPGP):**

`B0BA F819 B84B E96E CF22 B60C AD9C CEA6 3C3F BB30`

The public key is published as [`PGP_PUBLIC_KEY.asc`](PGP_PUBLIC_KEY.asc).

Verify the key's fingerprint before encrypting sensitive information. Encryption is optional and is not required to submit a report.

PGP encryption protects message contents when used correctly, but does not necessarily conceal email metadata, including sender and recipient addresses.

### Information requested

The reporting form is intended to collect:

- **Affected component:** Repository, package, version, endpoint, or system.
- **Summary:** A concise description of the suspected vulnerability.
- **Observed behavior:** What occurs and under which conditions.
- **Expected security behavior:** The property or protection potentially violated.
- **Reproduction:** Steps, prerequisites, or a minimal proof of concept.
- **Impact:** Demonstrated or plausible consequences, distinguished clearly.
- **Supporting evidence:** Relevant logs, screenshots, or references, appropriately redacted.
- **Suggested mitigation:** Potential corrections or workarounds, if known.

Reports should contain sufficient information for meaningful assessment without requiring reporters to supply a completed exploit, root-cause analysis, or proposed fix.

Do not include credentials, private keys, unnecessary personal information, or unrelated confidential material.

## 3. Responsible security research

Security research should be conducted within authorized boundaries and with care to avoid unintended consequences.

Researchers should:

- Limit testing to systems and resources they own or are expressly authorized to assess.
- Avoid disrupting service availability or degrading system performance.
- Avoid accessing, modifying, retaining, or disclosing information beyond what is necessary to establish the vulnerability.
- Stop testing when further investigation would require unauthorized access or create material operational impact.
- Report findings privately before public technical disclosure.
- Preserve sufficient evidence to support verification without collecting unnecessary sensitive information.

Public availability, discoverability, or technical accessibility does not constitute authorization to test a system.

This policy does not establish a bug bounty, grant permission for otherwise unauthorized activities, or independently create a legal safe harbor.

## 4. Handling vulnerability reports

Security reports should be evaluated according to their substance, technical evidence, and potential impact.

The handling process generally includes:

1. **Receipt:** Identify the affected project and preserve the report through an appropriate private channel.
2. **Assessment:** Determine whether the reported behavior is reproducible and whether it represents a security vulnerability.
3. **Impact evaluation:** Assess affected components, exploitability, potential consequences, and relevant dependencies.
4. **Remediation:** Develop and validate an appropriate correction or mitigation.
5. **Coordination:** Consider affected downstream users, maintainers, dependencies, and disclosure requirements.
6. **Disclosure:** Publish appropriate security information when doing so no longer creates an unreasonable exposure from an unresolved vulnerability.

Reports may be closed as unsubstantiated, duplicates, out of scope, or not security-relevant when supported by the findings.

A report should not be dismissed solely because the reporter lacks institutional affiliation, professional credentials, or an established relationship with the project.

### Response expectations

Means+Measures does not establish universal acknowledgment, remediation, or disclosure deadlines through this document.

Response and remediation priorities depend on the affected project, the nature of the vulnerability, its consequences, and available mitigation options.

Project-specific commitments, where adopted, should be documented separately.

## 5. Severity and prioritization

Security concerns should be evaluated using relevant technical evidence and the context in which an affected system operates.

Factors may include:

- Confidentiality, integrity, and availability impacts.
- Exploitability and prerequisites for exploitation.
- Exposure of affected components.
- Whether exploitation has been observed.
- Sensitivity of affected information.
- Scope and reversibility of potential consequences.
- Availability and effectiveness of mitigations.
- Effects on users who depend on the system for access to essential functions or information.

Established frameworks, including the Common Vulnerability Scoring System (CVSS), may inform assessments where appropriate.

Severity classifications should distinguish demonstrated impacts from plausible but unverified consequences.

## 6. Remediation and disclosure

Verified vulnerabilities should be addressed through corrections or mitigations appropriate to their severity and circumstances.

Remediation may involve source changes, configuration changes, dependency updates, access restrictions, credential rotation, or operational controls.

Where appropriate, disclosure may use GitHub Security Advisories, coordinated vulnerability disclosure processes, or other project-specific mechanisms.

Public advisories should communicate:

- The affected component and versions, where known.
- The nature and consequences of the vulnerability.
- Available fixes or mitigations.
- Relevant identifiers and references, where assigned.
- Material limitations or unresolved conditions.

Disclosure should provide actionable information without unnecessarily exposing confidential data or creating additional risk.

Public reporting may be coordinated with researchers and affected parties, subject to applicable obligations and the circumstances of the vulnerability.

## 7. Dependencies and supply-chain security

Security includes the integrity of software dependencies, development workflows, build processes, and distribution mechanisms.

Contributors and maintainers should consider:

- The provenance and maintenance status of dependencies.
- Dependency vulnerabilities and available updates.
- The permissions granted to automation and integrations.
- The integrity of build and release artifacts.
- The handling of credentials and deployment secrets.
- The consequences of introducing or removing external dependencies.

Automated security tools may assist detection and maintenance, but their findings require appropriate interpretation and verification.

A passing automated scan does not establish that a system is free of vulnerabilities.

## 8. Credentials and sensitive information

Credentials, private keys, authentication tokens, and other secrets must not be intentionally committed to public repositories.

If potentially sensitive information is exposed:

1. Report the exposure through the designated private vulnerability reporting process or encrypted reporting email.
2. Identify the affected credentials or information without reproducing unnecessary sensitive contents.
3. Revoke or rotate compromised credentials where authorized and applicable.
4. Assess whether additional access, disclosure, or remediation is necessary.

Removing a secret from a file does not necessarily remove it from version history, caches, forks, or other copies. Credential invalidation and impact assessment may therefore remain necessary.

## 9. Security and accessibility

Security controls should be evaluated for both protective effectiveness and their effects on legitimate access.

Authentication, authorization, identity verification, abuse prevention, and account recovery mechanisms can introduce barriers when they depend on inaccessible interfaces, unavailable resources, or assumptions about users' circumstances.

Security requirements should not be abandoned to achieve accessibility, nor should accessibility concerns be dismissed solely because a control is described as a security measure.

Both objectives should inform the design and evaluation of appropriate controls.

## 10. Accountability and continuous improvement

Security outcomes should be evaluated against evidence of actual system behavior, not merely the presence of policies or controls.

Identified failures, vulnerabilities, and near misses may warrant changes to implementation, testing, documentation, dependencies, or operational practices.

Relevant findings and remediation decisions should preserve sufficient provenance for future review without exposing information that must remain confidential.

The standards applied to external systems also apply to Means+Measures projects.

## Policy maintenance

This policy may be revised through the established contribution and governance processes.

Project maintainers may document additional technical requirements or reporting procedures applicable to their repositories.

Such procedures should identify any materially different reporting channels, supported versions, or security commitments.

---

**Security reporting:** Use GitHub's private vulnerability reporting form or email **privacy-contact@mail.meansandmeasures.com**. OpenPGP encryption is supported. Never place exploit details or sensitive evidence in a public GitHub issue.