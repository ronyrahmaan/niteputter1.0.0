# Security Policy

## Supported Versions

We actively support and provide security updates for the following versions:

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |

## Reporting a Vulnerability

We take the security of NitePutter seriously. If you discover a security vulnerability, please follow these guidelines:

### How to Report

**Do NOT create a public GitHub issue for security vulnerabilities.**

Instead, please report security issues via email to:
- **Security Team**: security@niteputter.com
- **Subject Line**: [SECURITY] Brief description of the issue

### What to Include

Please provide as much information as possible to help us understand and resolve the issue quickly:

1. **Description**: Clear description of the vulnerability
2. **Impact**: Potential impact and who might be affected
3. **Reproduction**: Step-by-step instructions to reproduce the issue
4. **Environment**: Device type, OS version, app version
5. **Proof of Concept**: If possible, include a minimal example
6. **Suggested Fix**: If you have ideas for fixing the issue

### Response Timeline

We are committed to responding to security reports promptly:

- **Initial Response**: Within 24 hours of report receipt
- **Investigation Update**: Within 72 hours with preliminary findings
- **Resolution Timeline**: Severity-dependent, typically 7-30 days

### Severity Classification

We classify security issues based on potential impact:

#### Critical (24-48 hours)
- Remote code execution
- Data breach affecting user credentials
- Payment system vulnerabilities

#### High (3-7 days)
- Privilege escalation
- Authentication bypass
- Sensitive data exposure

#### Medium (7-14 days)
- Information disclosure
- Denial of service
- Session management issues

#### Low (14-30 days)
- Security misconfigurations
- Minor information leaks
- Best practice violations

### Security Measures

#### Data Protection
- All user data encrypted at rest and in transit
- Payment information handled exclusively by Stripe (PCI DSS compliant)
- Personal information protected according to privacy regulations
- Regular security audits and penetration testing

#### Application Security
- Secure coding practices and regular code reviews
- Input validation and sanitization
- Protection against common vulnerabilities (OWASP Top 10)
- Regular dependency updates and vulnerability scanning

#### Infrastructure Security
- Secure cloud infrastructure with Supabase
- Environment-based configuration management
- Access controls and authentication systems
- Monitoring and logging for security events

#### Mobile Security
- Certificate pinning for API communications
- Secure storage for sensitive data
- Biometric authentication where supported
- App transport security (ATS) compliance

### Disclosure Policy

#### Coordinated Disclosure
1. **Investigation**: We investigate and verify the reported issue
2. **Fix Development**: We develop and test a security fix
3. **Release**: We release the fix in a new version
4. **Public Disclosure**: After users have had time to update (typically 30 days)

#### Recognition
We appreciate security researchers who help improve our security:
- Security researchers will be credited in our security advisory (with permission)
- We may provide recognition on our website or documentation
- For significant findings, we may offer bug bounty rewards

### Security Best Practices for Users

#### For End Users
- Keep the app updated to the latest version
- Use strong, unique passwords for your account
- Enable biometric authentication if available
- Be cautious when connecting to public Wi-Fi networks
- Report suspicious activity immediately

#### For Developers
- Follow secure coding guidelines in our documentation
- Keep dependencies updated
- Use environment variables for sensitive configuration
- Implement proper error handling to prevent information leakage
- Regular security testing of new features

### Legal

This security policy is designed to protect both NitePutter and security researchers. We commit to:

- Not pursue legal action against researchers who follow this policy
- Work in good faith to resolve security issues
- Provide recognition for responsible disclosure

### Contact Information

- **Security Email**: security@niteputter.com
- **General Support**: support@niteputter.com
- **Business Inquiries**: contact@niteputter.com

### Updates

This security policy may be updated periodically. The latest version will always be available in this repository.

Last updated: December 18, 2024