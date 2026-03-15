# Changelog Generator Skill

A global AI agent skill for generating, managing, and maintaining standard `CHANGELOG.md` files in your projects.

## Overview

**What pain points does it solve?**
Have you ever struggled to remember what changes you or your AI agent made today? Tired of scrolling through chat logs to summarize your work? With `changelog-generator`, you no longer need to manually write down what was done. The agent automatically acts as your scribe, aggregating your daily updates and formatting them perfectly into your project's `CHANGELOG.md`.

This skill allows your AI assistant to automatically detect updates, feature additions, or bug fixes, and categorize them into a standardized format. It strictly follows:
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
