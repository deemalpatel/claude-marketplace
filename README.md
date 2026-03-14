# Claude Marketplace Plugins

This repository contains a small Claude plugin marketplace definition and four local plugins:

- `daily-summary`
- `optimization-review`
- `security-review`
- `ui-ux-critique`

The marketplace manifest lives at [`.claude-plugin/marketplace.json`](/Users/deemalpatel/Documents/claude-marketplace/.claude-plugin/marketplace.json) and points Claude-compatible tooling at the plugins stored under [`plugins/`](/Users/deemalpatel/Documents/claude-marketplace/plugins).

## Repository Structure

```text
.claude-plugin/marketplace.json
plugins/
  daily-summary-plugin/
  optimization-review-plugin/
  security-review-plugin/
  ui-ux-critique-plugin/
```

Each plugin includes:

- a `.claude-plugin/plugin.json` manifest
- one skill under `skills/.../SKILL.md`

## Included Plugins

### Daily Summary

Source: [`plugins/daily-summary-plugin`](/Users/deemalpatel/Documents/claude-marketplace/plugins/daily-summary-plugin)

Provides a skill for summarizing daily development work, feature progress, or code changes.

### Optimization Review

Source: [`plugins/optimization-review-plugin`](/Users/deemalpatel/Documents/claude-marketplace/plugins/optimization-review-plugin)

Provides a skill focused on identifying code paths, rendering behavior, or implementation details that can be improved for performance.

### Security Review

Source: [`plugins/security-review-plugin`](/Users/deemalpatel/Documents/claude-marketplace/plugins/security-review-plugin)

Provides a skill for reviewing code for vulnerabilities, unsafe patterns, and general security risks.

### UI / UX Critique

Source: [`plugins/ui-ux-critique-plugin`](/Users/deemalpatel/Documents/claude-marketplace/plugins/ui-ux-critique-plugin)

Provides a skill for evaluating interface quality, usability, and overall visual polish.

## Marketplace Manifest

The marketplace manifest declares:

- marketplace name: `my-plugins`
- owner: `Deemal Patel`
- plugin source paths relative to the repository root

If you add another plugin, update [`.claude-plugin/marketplace.json`](/Users/deemalpatel/Documents/claude-marketplace/.claude-plugin/marketplace.json) with a new entry in the `plugins` array and add the plugin folder under [`plugins/`](/Users/deemalpatel/Documents/claude-marketplace/plugins).

## Development Notes

To keep the marketplace consistent:

- use one plugin directory per skill package
- keep plugin metadata in `.claude-plugin/plugin.json`
- store the actual instructions in `skills/<skill-name>/SKILL.md`
- keep descriptions short and specific so the marketplace is easy to scan

## Next Improvements

Useful follow-up additions for this repository:

- installation instructions for the target Claude environment
- example prompts for each skill
- versioning and release notes for plugin changes
- tests or validation scripts for manifest consistency
