# 🔌 Trae Integration

The Agency agents are converted into Markdown rule files compatible with Trae.

## Installation

### Project-Scoped (Recommended)

To use these agents within a specific project, run the installer from that project's root:

```bash
cd /path/to/your/project
/path/to/agency-agents/scripts/install.sh --tool trae
```

This will copy all 120 agents into `.trae/rules/`.

### Global-Scoped

The installer also automatically attempts to install agents to `~/.trae/rules/` for global availability across all your Trae projects.

## Usage

Once installed, Trae automatically scans the `.trae/rules/` directory. You can guide the AI by referencing specific agents or simply letting it follow the established rules for:

- Code Style & Standards
- Architecture Patterns
- Testing Procedures
- Personality & Communication Tone

## Regenerating

If you add new agents to the repo, regenerate the Trae integration files first:

```bash
./scripts/convert.sh --tool trae
```
