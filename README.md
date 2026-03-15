# Changelog Generator Skill

A global AI agent skill for generating, managing, and maintaining standard `CHANGELOG.md` files in your projects.

## Overview

This skill allows an AI assistant to automatically detect updates, feature additions, or bug fixes, and correctly categorize them into a standardized `CHANGELOG.md` in the project root. It follows the principles of:
1. [Keep a Changelog](https://keepachangelog.com/)
2. [Semantic Versioning](https://semver.org/)

## Features

- **Auto-Initialization**: Creates a standardized `CHANGELOG.md` if one doesn't exist.
- **Smart Categorization**: Groups changes into `Added`, `Changed`, `Deprecated`, `Removed`, `Fixed`, and `Security`.
- **Version Management**: Uses Semantic Versioning to determine major, minor, or patch numbers dynamically.
- **Proactive Logging**: Keeps track of prior context and automatically drafts the changelog update.

## Installation

Clone this repository into your AI agents' skills directory.

```bash
git clone https://github.com/CalvinQin/changelog-generator.git ~/.agents/skills/changelog-generator
或者
git clone https://github.com/CalvinQin/changelog-generator.git ~/.gemini/antigravity/skills/changelog-generator
```

Then register the skill inside your `SKILLS_LOG.md` or dynamically attach it when starting your agent environment.

## Requirements

None. Purely relies on the AI assistant's ability to read and write to the local file system.

## License

MIT
