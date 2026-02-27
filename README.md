# Claude Skills Pack JA

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/manabuozato/claude-skills-pack-ja.svg?style=social)](https://github.com/manabuozato/claude-skills-pack-ja/stargazers)

A curated collection of **Claude.ai skills** designed for Japanese business workflows — meeting minutes, daily reports, morning routines, and more.

## What is this?

Claude.ai allows users to upload custom instructions (called "skills") as Project Knowledge files. These skills act as reusable prompts that trigger automatically when Claude detects relevant context in your conversation.

**This repository** provides ready-to-use skill files (`.md`) tailored for Japanese business environments. Each skill understands Japanese business customs — keigo, meeting structures, wareki dates, and more.

## Skills

| Skill | Description | Target User |
|-------|-------------|-------------|
| [Meeting Minutes](skills/meeting-minutes/SKILL.md) | Auto-generate structured meeting minutes from transcripts | Anyone who attends meetings |
| [Daily Report](skills/daily-report/SKILL.md) | Compile daily reports from calendar and notes | Office workers, managers |
| [Morning Setup](skills/morning-setup/SKILL.md) | Morning routine: calendar, email, task organization | Anyone starting their workday |
| [Notion Integration](skills/notion-integration/SKILL.md) | Notion MCP templates for TODO, daily reports, projects | Notion users with MCP enabled |
| [Email Triage](skills/email-triage/SKILL.md) | Multi-account email triage with priority classification | Busy professionals |

## Quick Start

1. **Download** the `SKILL.md` file for the skill you want
2. **Open** [Claude.ai](https://claude.ai) and go to your Project
3. **Upload** the `SKILL.md` file to Project Knowledge
4. **Start chatting** — the skill activates automatically when it detects trigger phrases

That's it. No coding, no API keys, no setup.

### Example

After uploading `meeting-minutes/SKILL.md`, just paste a meeting transcript and say:

> 議事録にまとめて

Claude will automatically generate structured meeting minutes in Japanese business format.

## Skill Details

### Meeting Minutes (`meeting-minutes/`)

Converts raw meeting transcripts (from Tactiq, Otter.ai, manual notes, etc.) into structured minutes with:
- Meeting metadata (name, date, attendees)
- Discussion points with speaker attribution
- Decisions and action items with assignees and deadlines
- Keigo normalization and desu/masu to de-aru conversion

### Daily Report (`daily-report/`)

Compiles your daily report by pulling together:
- Calendar events and meeting outcomes
- Task completions categorized by project
- Tomorrow's plan and priorities
- Reflections and concerns

### Morning Setup (`morning-setup/`)

A morning routine assistant that:
- Updates today's date context
- Checks your calendar for today's schedule
- Summarizes unread emails
- Organizes tasks by priority
- Sets your focus for the day

### Notion Integration (`notion-integration/`)

Templates for Claude + Notion MCP integration:
- TODO management patterns
- Daily report database updates
- Project tracking workflows

### Email Triage (`email-triage/`)

Multi-account email management:
- Checks unread across all accounts
- Auto-classifies by urgency and importance
- Generates reply drafts in appropriate tone

## Born from daily use

These are not theoretical templates. Every skill in this pack is something the author actually uses in daily work — managing meetings, writing reports, organizing mornings, and staying on top of email across multiple accounts. They have been refined through months of real-world use in Japanese business settings.

If something feels practical and opinionated, that's intentional.

## Examples

See the [examples/](examples/) directory for sample inputs and outputs:
- [Meeting Minutes Example](examples/meeting-minutes-example.md)
- [Daily Report Example](examples/daily-report-example.md)
- [Morning Setup Example](examples/morning-setup-example.md)

## Documentation

- [Installation Guide](docs/installation.md) — How to install skills in Claude.ai
- [Customization Guide](docs/customization.md) — How to adapt skills to your workflow

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a pull request.

We especially welcome:
- New skills for Japanese business workflows
- Translations and localization improvements
- Bug fixes and documentation improvements

## License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

## Author

**Manabu Ozato** ([@manabuozato](https://github.com/manabuozato))
Producer / Researcher, PhD candidate at JAIST (Japan Advanced Institute of Science and Technology)

---

[日本語版 README はこちら](README.ja.md)
