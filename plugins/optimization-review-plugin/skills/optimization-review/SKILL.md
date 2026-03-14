# Claude Skill: Performance & Optimization Review

## Goal
Identify performance bottlenecks, inefficient rendering, slow processing logic, and opportunities for architectural optimization.

## Scope
Analyze the entire system including:

- Frontend rendering
- API requests
- Backend processing
- Database queries
- State management
- Caching
- Build configuration
- Network behavior

## Performance Review Checklist

### Rendering Performance
Look for:
- Unnecessary component re-renders
- Expensive logic inside render functions
- Missing memoization
- Large component trees
- Inefficient state updates
- Unoptimized lists or loops

### Network Performance
Identify:
- Duplicate API calls
- Unnecessary requests
- Large payloads
- Missing caching
- Inefficient polling

### Backend Processing
Check for:
- N+1 queries
- Inefficient database queries
- Missing indexes
- Heavy work inside request handlers
- Blocking synchronous work
- Repeated expensive computations

### Database Performance
Review:
- Slow queries
- Missing indexes
- Large unfiltered queries
- Excessive joins
- Redundant data fetching

### Memory Usage
Look for:
- Memory leaks
- Large objects stored unnecessarily
- Unbounded caches
- Objects retained longer than needed

### CPU Usage
Identify:
- Expensive loops
- Repeated heavy computations
- Inefficient algorithms
- Excessive data transformations

### Caching Opportunities
Check for:
- Missing API caching
- Missing query caching
- Missing CDN usage
- Opportunities for memoization

### Build & Bundle Optimization
Look for:
- Large bundles
- Unused dependencies
- Missing code splitting
- Inefficient asset loading

### Code Efficiency
Identify:
- Duplicated logic
- Inefficient patterns
- Overly complex functions
- Tight coupling affecting performance

## Output Format

# Performance Audit

## Major Bottlenecks
- description
- location
- reason for slowdown
- suggested optimization

## Rendering Issues
- description
- location
- improvement suggestion

## Backend Performance Risks
- description
- location
- recommended fix

## Optimization Opportunities
- performance improvement suggestion

## Quick Wins
Small improvements that significantly increase performance

## Behavior Rules

- Focus on real performance problems
- Prioritize issues affecting rendering or request latency
- Avoid style-only suggestions
- Provide actionable optimization steps
- Explain why the change improves performance

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