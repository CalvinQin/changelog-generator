---
name: changelog-generator
description: A global skill to automatically generate, maintain, and format project CHANGELOG.md files and manage version numbers based on Semantic Versioning. Use when the user asks to update the changelog, bump version, create release notes, record project updates, or maintain version history in the project root.
---

# Changelog Generator

When invoked to update the project's changelog, follow these strict rules to ensure standardized logging practices across all projects:

## 1. Locate or Initialize
- Locate the `CHANGELOG.md` in the user's current project root.
- If it doesn't exist, create it following the [Keep a Changelog](https://keepachangelog.com/) format and [Semantic Versioning](https://semver.org/).

## 2. Version Management
- If the user specifies a version bump (major/minor/patch) or simply asks to log changes for the day, calculate or define the new version based on the current version structure.
- Always include the current date `[YYYY-MM-DD]` alongside the version number in the heading (e.g., `## [3.1.0] - 2026-03-16`).
- If starting a new project without prior version semantics, assume a baseline (like `0.1.0` or `1.0.0`) unless instructed otherwise by the user.

## 3. Categorization
Organize changes into the following groups (do not use empty sections):
- `Added` for new features or documentation.
- `Changed` for changes in existing functionality.
- `Deprecated` for soon-to-be removed features.
- `Removed` for now removed features.
- `Fixed` for any bug fixes or performance optimizations.
- `Security` in case of vulnerabilities.

## 4. Formatting Rules
- Always prepend the new version block at the top of the version history section (below the "Unreleased" header if one is used).
- Use clear, bulleted statements describing actual changes. DO NOT include vague technical jargon unless relevant.
- Write the changes in **Chinese** if the project is predominantly using Chinese (like TradeFlow) or if the user's prompt is in Chinese, else default to English.

## 5. Proactivity
- Actively infer changes from your recent conversational context or task history if the user says "Record what we just did to the changelog".
- Ensure you commit or write back to the `CHANGELOG.md` automatically, alleviating the user from manual documentation.
