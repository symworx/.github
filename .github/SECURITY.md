# Security Policy

## Supported versions

Security fixes are generally applied to the default branch of each actively
maintained SymWorx repository. If a project publishes versioned releases,
prefer the latest release line unless maintainers state otherwise.

## Reporting a vulnerability

**Do not** open a public issue for security vulnerabilities.

Please report vulnerabilities privately using one of these methods:

1. **GitHub Security Advisories** (preferred)  
   On [symworx/symworx](https://github.com/symworx/symworx) when the
   repository is available: **Security → Report a vulnerability**.

2. **Organization contact**  
   Contact an organization owner via GitHub if private reporting is unavailable
   or the monorepo is not yet public.

Include as much detail as you can:

- Affected repository and version / commit
- Impact and attack scenario
- Steps to reproduce or a proof of concept
- Any known workarounds

## What to expect

- We will acknowledge receipt when we can and keep the conversation private
  until a fix is ready or the report is determined not to be a vulnerability.
- We may ask for more information or collaboration on a fix.
- Coordinated disclosure is preferred; please do not publish exploit details
  until maintainers have had a reasonable chance to release a patch.

## Scope

In scope: code, dependencies, and configuration in the
[symworx/symworx](https://github.com/symworx/symworx) monorepo that could lead
to unauthorized access, data exposure, privilege escalation, or remote code
execution.

Out of scope: social engineering against individuals, denial-of-service against
GitHub.com itself, and issues in third-party projects not under our control.
