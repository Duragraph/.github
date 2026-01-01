# Security Policy

## Supported Versions

We release patches for security vulnerabilities in the following versions:

| Version | Supported          |
| ------- | ------------------ |
| latest  | :white_check_mark: |
| < 1.0   | :x:                |

## Reporting a Vulnerability

We take security seriously at DuraGraph. If you discover a security vulnerability, please report it responsibly.

### How to Report

**Please do NOT report security vulnerabilities through public GitHub issues.**

Instead, please report them via email to:

**security@duragraph.dev**

Include the following information in your report:

1. **Description** of the vulnerability
2. **Steps to reproduce** the issue
3. **Affected versions**
4. **Potential impact**
5. **Any suggested fixes** (optional)

### What to Expect

- **Acknowledgment**: We will acknowledge receipt of your report within 48 hours
- **Assessment**: We will investigate and assess the vulnerability within 7 days
- **Updates**: We will keep you informed of our progress
- **Resolution**: We aim to resolve critical vulnerabilities within 30 days
- **Credit**: We will credit you in the security advisory (unless you prefer to remain anonymous)

### Scope

This security policy applies to:

- [duragraph](https://github.com/Duragraph/duragraph) - Core API server
- [duragraph-python](https://github.com/Duragraph/duragraph-python) - Python SDK
- [duragraph-go](https://github.com/Duragraph/duragraph-go) - Go SDK
- [duragraph-studio](https://github.com/Duragraph/duragraph-studio) - Interactive UI

### Out of Scope

- Vulnerabilities in third-party dependencies (please report these to the respective maintainers)
- Social engineering attacks
- Physical security issues
- Denial of service attacks

## Security Best Practices

When using DuraGraph:

1. **Keep dependencies updated** - Regularly update to the latest versions
2. **Use environment variables** - Never hardcode API keys or secrets
3. **Enable authentication** - Use JWT authentication in production
4. **Use TLS** - Always use HTTPS in production environments
5. **Limit permissions** - Follow the principle of least privilege
6. **Monitor logs** - Review logs for suspicious activity

## Security Advisories

Security advisories will be published on:

- [GitHub Security Advisories](https://github.com/Duragraph/duragraph/security/advisories)
- Release notes

## Contact

For security-related questions that are not vulnerabilities, you can reach us at:

- Email: security@duragraph.dev
- GitHub Discussions: https://github.com/orgs/Duragraph/discussions

Thank you for helping keep DuraGraph secure!
