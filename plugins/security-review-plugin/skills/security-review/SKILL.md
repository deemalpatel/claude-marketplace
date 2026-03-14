# Claude Skill: Security Review

## Goal
Perform a deep security audit of the codebase to identify vulnerabilities, unsafe patterns, and configuration risks.

## Scope
Review all parts of the system including:

- API routes
- Backend services
- Database queries
- Authentication and authorization logic
- File uploads
- External integrations
- Environment variable usage
- Infrastructure configuration
- Logging and error handling

## Security Review Checklist

### Input Validation
Look for:
- Missing input validation
- Missing schema validation
- Improper sanitization
- Unsafe parsing
- Trusting client-side data

### Injection Vulnerabilities
Check for:
- SQL Injection
- NoSQL Injection
- Command Injection
- Template Injection
- Unsafe query construction

### Authentication
Verify:
- Proper authentication checks
- Session handling safety
- JWT verification and expiration
- Token leakage
- Password storage security

### Authorization
Look for:
- Missing role checks
- Privilege escalation risks
- Broken access control
- Missing ownership checks
- Insecure direct object references (IDOR)

### Sensitive Data Exposure
Identify:
- Hardcoded secrets
- API keys in source code
- Logging of sensitive information
- Improper environment variable handling
- Unencrypted sensitive data

### API Security
Review:
- Missing rate limiting
- Missing request validation
- Overly permissive endpoints
- Missing authentication middleware
- Unsafe query parameters

### File Handling
Check for:
- Unsafe file uploads
- Missing file type validation
- Path traversal vulnerabilities
- Arbitrary file writes
- Lack of file size limits

### Dependency Risks
Look for:
- Known vulnerable packages
- Unmaintained libraries
- Unsafe dependencies

### Configuration Issues
Verify:
- Debug mode disabled in production
- Proper CORS configuration
- Secure HTTP headers
- Proper environment isolation

## Output Format

# Security Audit

## Critical Vulnerabilities
- description
- location
- why it is dangerous
- recommended fix

## Security Risks
- description
- location
- recommended fix

## Hardening Recommendations
- security improvement suggestion

## Quick Fixes
Small changes that significantly improve security

## Behavior Rules

- Focus on real vulnerabilities, not style issues
- Prioritize critical security risks
- Provide file locations when possible
- Explain why each issue is dangerous
- Suggest concrete fixes

## Fresh Analysis Requirement

Always perform a **fresh analysis of the current codebase** when running this skill.

Do NOT rely on:
- previous analyses
- cached reasoning
- earlier summaries
- previously reported issues

Before producing any findings:

1. Re-scan the relevant files in the repository.
2. Re-evaluate the current implementation.
3. Confirm that each issue still exists in the latest code.
4. Ignore previously reported issues unless they are verified again in the current code.

If the code has changed since the last review, treat the review as **a completely new audit**.

Only report findings that are **confirmed in the current codebase**.

## Review Procedure

Follow this process every time:

1. Discover all relevant files in the repository.
2. Read the files directly before making conclusions.
3. Analyze the actual implementation.
4. Only then produce the audit report.

Never assume behavior without reading the source code.

Always assume the code may have changed since the last run.

Never trust previous conclusions without verifying them again.