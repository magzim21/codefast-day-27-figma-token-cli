# Codefast Day 27 · Figma Token CLI

## Mission
- Provide a CLI for syncing Figma tokens across repos, emitting change logs, and GitHub check outputs.

## Implementation Checklist
1. Support commands for pull, diff, publish, and validate operations with configuration file.
2. Output Markdown changelog summarizing token updates, breaking changes, and impacted components.
3. Integrate with GitHub Checks API, annotating PRs with token diffs.
4. Cache responses locally to respect Figma rate limits and support offline simulation.

## Telemetry & QA
- Track command runtimes and failure rates via Datadog statsd.
- Unit test command handlers and golden-file diff outputs.

## Deliverables
- README with installation steps, command reference, and CI usage examples.
- Contribution guide for adding new exporters or token formats.
