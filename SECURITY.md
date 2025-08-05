# Security Policy

## Supported Versions

We release patches to fix security vulnerabilities. Which versions are eligible for such patches depends on the CVSS v3.0 Rating:

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |

## Reporting a Vulnerability

We take the security of our add-ons seriously. If you believe you have found a security vulnerability, please report it to us as described below.

**Please do not report security vulnerabilities through public GitHub issues.**

Instead, please report them via email to [security@example.com](mailto:security@example.com).

You should receive a response within 48 hours. If for some reason you do not, please follow up via email to ensure we received your original message.

Please include the requested information listed below (as much as you can provide) to help us better understand the nature and scope of the possible issue:

- Type of issue (buffer overflow, SQL injection, cross-site scripting, etc.)
- Full paths of source file(s) related to the vulnerability
- The location of the affected source code (tag/branch/commit or direct URL)
- Any special configuration required to reproduce the issue
- Step-by-step instructions to reproduce the issue
- Proof-of-concept or exploit code (if possible)
- Impact of the issue, including how an attacker might exploit it

This information will help us triage your report more quickly.

## Preferred Languages

We prefer all communications to be in English.

## Policy

We take security seriously and will make every effort to promptly address any reported issues. We appreciate your efforts to responsibly disclose your findings, and will make every effort to acknowledge your contributions.

## Security Best Practices

When using our add-ons:

1. **Keep Home Assistant updated** to the latest version
2. **Use strong passwords** for any authentication
3. **Limit network access** to only necessary ports
4. **Monitor logs** for suspicious activity
5. **Backup configurations** regularly
6. **Use HTTPS** when possible for external access
7. **Review add-on permissions** before installation

## Security Considerations for Add-ons

Our add-ons are designed with security in mind:

- **Containerized execution** for isolation
- **Minimal permissions** principle
- **Network access control** where possible
- **Regular security updates** for dependencies
- **Input validation** and sanitization
- **Secure defaults** for configurations

## Disclosure Policy

When we receive a security bug report, we will:

1. Confirm the problem and determine the affected versions
2. Audit code to find any similar problems
3. Prepare fixes for all supported versions
4. Release new versions with the fixes
5. Publicly announce the vulnerability

## Credits

We would like to thank all security researchers and users who responsibly disclose vulnerabilities to us. Your contributions help make our add-ons more secure for everyone. 