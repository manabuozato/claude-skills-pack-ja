# Contributing to Claude Skills Pack JA

Thank you for your interest in contributing! This project thrives on community input, especially from people who use Claude.ai in Japanese business settings.

## How to Contribute

### Reporting Issues

- Use the [Bug Report](https://github.com/manabuozato/claude-skills-pack-ja/issues/new?template=bug_report.md) template for skill malfunctions
- Use the [Feature Request](https://github.com/manabuozato/claude-skills-pack-ja/issues/new?template=feature_request.md) template for new skill ideas

### Submitting a New Skill

1. **Fork** the repository
2. **Create a branch**: `git checkout -b skill/your-skill-name`
3. **Create the skill directory**: `skills/your-skill-name/SKILL.md`
4. **Add an example** (optional but encouraged): `examples/your-skill-name-example.md`
5. **Update README.md** and **README.ja.md** with your skill in the skills table
6. **Submit a Pull Request** using the PR template

### Skill File Requirements

Every `SKILL.md` must include:

1. **Description block** at the top with:
   - Skill name (Japanese and English)
   - Trigger conditions (what phrases activate the skill)
   - Brief description of what the skill does

2. **Steps** numbered and clearly structured

3. **Output format template** showing the expected output structure

4. **Customization points** clearly marked with `<!-- CUSTOMIZE -->` comments

5. **Japanese business context** considerations (keigo, formatting, etc.)

### Code Style

- Markdown files should use ATX-style headers (`#`, `##`, `###`)
- Use fenced code blocks with language identifiers
- Keep lines under 120 characters where possible
- Use consistent Japanese formatting (full-width punctuation in Japanese text)

### Commit Messages

- Use conventional commit format: `feat:`, `fix:`, `docs:`, `chore:`
- Write commit messages in English
- Example: `feat: add invoice-generation skill`

### Pull Request Process

1. Ensure your skill works correctly when uploaded to Claude.ai Project Knowledge
2. Include before/after examples if applicable
3. Update documentation as needed
4. Request review from the maintainer

## Skill Design Principles

When creating a new skill, follow these principles:

- **Practical first**: Skills should solve real daily problems
- **Japanese context**: Consider keigo levels, date formats (wareki), naming conventions
- **Trigger-based**: Skills should activate on natural Japanese phrases
- **Structured output**: Every skill should produce consistently formatted output
- **Customizable**: Mark points where users might want to adjust behavior

## Questions?

Feel free to open an issue with the "question" label if you need help or have ideas to discuss.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
