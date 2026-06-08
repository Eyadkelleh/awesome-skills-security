# Awesome Security Skills: Security Collection

[![skills.sh](https://skills.sh/b/Eyadkelleh/awesome-skills-security)](https://skills.sh/Eyadkelleh/awesome-skills-security)

A curated collection of security testing resources packaged as agent skills, available on [skills.sh](https://skills.sh/)

**Repository:** [Eyadkelleh/awesome-skills-security](https://github.com/Eyadkelleh/awesome-skills-security) · **skills.sh:** [Eyadkelleh/awesome-skills-security](https://skills.sh/Eyadkelleh/awesome-skills-security)

## Overview

This repository contains a curated collection of security testing resources from [SecLists](https://github.com/danielmiessler/SecLists) packaged as [Agent Skills](https://agentskills.io) for use with Claude Code, Cursor, Codex, and [60+ other supported agents](https://skills.sh/). These skills provide instant access to essential wordlists, payloads, patterns, and web shells for authorized security testing, penetration testing, CTF competitions, and security research.

The goal of this project is to provide organized, immediately accessible security testing resources that integrate seamlessly with AI agent workflows for:

- Authorized penetration testing and security assessments
- Bug bounty program research
- CTF competition problem solving
- Security tool development and testing
- Educational security demonstrations
- Vulnerability research in controlled environments

## Quick Start

### Install from skills.sh (Recommended)

The easiest way to get started is to install from the [skills.sh](https://skills.sh/) directory using the open agent skills CLI:

```bash
# List all available skills in this repository
npx skills add Eyadkelleh/awesome-skills-security --list

# Install all 7 security skills
npx skills add Eyadkelleh/awesome-skills-security --skill '*' -y

# Install specific skills
npx skills add Eyadkelleh/awesome-skills-security --skill security-fuzzing --skill llm-testing -y

# Install to a specific agent (e.g. Cursor or Claude Code)
npx skills add Eyadkelleh/awesome-skills-security -a cursor -y
npx skills add Eyadkelleh/awesome-skills-security -a claude-code -y

# Install globally (available across all projects)
npx skills add Eyadkelleh/awesome-skills-security --skill '*' -g -y
```

Browse and discover this collection on skills.sh: [skills.sh/Eyadkelleh/awesome-skills-security](https://skills.sh/Eyadkelleh/awesome-skills-security)

### Verify Installation

After installing, verify the skills are available:

```bash
# List installed skills
npx skills list

# Or ask your agent to use a skill
"Use the security-fuzzing skill to show me SQL injection payloads"
```

### What You Get

Once installed, you'll have access to:
- **7 Security Skill Categories**: Fuzzing, Passwords, Patterns, Payloads, Usernames, Web-shells, LLM Testing
- **Curated SecLists Content**: Essential wordlists and payloads for security testing
- **LLM Security Testing**: Comprehensive AI/ML security testing prompts and methodologies

### Troubleshooting

**"No skills found"**
- Ensure you're using the correct repo: `Eyadkelleh/awesome-skills-security`
- Run `npx skills add Eyadkelleh/awesome-skills-security --list` to verify discovery
- Each `SKILL.md` must have valid YAML frontmatter with `name` (lowercase, hyphens) and `description`

**"Skill not loading in agent"**
- Verify the skill was installed to the correct agent directory (e.g. `.cursor/skills/`)
- Try reinstalling: `npx skills add Eyadkelleh/awesome-skills-security --skill <name> -y`
- Check your agent's documentation for skill loading requirements

**Need help?**
- Open an issue on [GitHub](https://github.com/Eyadkelleh/awesome-skills-security/issues)
- Check the [skills.sh directory](https://skills.sh/) and [Agent Skills spec](https://agentskills.io)

## Available Skills

All skills live under `skills/` and are discoverable by the [skills.sh CLI](https://skills.sh/). Each skill has a `SKILL.md` with `name` and `description` frontmatter.

| Skill ID | Description | Install command |
|:---------|:------------|:----------------|
| `security-fuzzing` | SQL, NoSQL, command injection, and LDAP fuzzing payloads | `npx skills add Eyadkelleh/awesome-skills-security --skill security-fuzzing -y` |
| `security-passwords` | Curated password wordlists for authorized credential testing | `npx skills add Eyadkelleh/awesome-skills-security --skill security-passwords -y` |
| `security-patterns` | API keys, credit cards, emails, and sensitive data patterns | `npx skills add Eyadkelleh/awesome-skills-security --skill security-patterns -y` |
| `security-payloads` | XSS, XXE, template injection, and file upload payloads | `npx skills add Eyadkelleh/awesome-skills-security --skill security-payloads -y` |
| `security-usernames` | Common username wordlists for enumeration | `npx skills add Eyadkelleh/awesome-skills-security --skill security-usernames -y` |
| `security-webshells` | Web shell samples for detection and defensive testing | `npx skills add Eyadkelleh/awesome-skills-security --skill security-webshells -y` |
| `llm-testing` | LLM bias, data leakage, alignment, and adversarial testing prompts | `npx skills add Eyadkelleh/awesome-skills-security --skill llm-testing -y` |

### Fuzzing (`security-fuzzing`)
**Essential fuzzing payloads for vulnerability testing**
- SQL injection testing payloads
- Command injection patterns
- NoSQL injection vectors
- LDAP injection strings
- Special character fuzzing
- Authentication bypass patterns

### Passwords (`security-passwords`)
**Curated password lists for authorized credential testing**
- 500 worst passwords
- 10K most common passwords
- 100K NCSC password list
- Dark web breach compilations
- Probable password variations

### Pattern-Matching (`security-patterns`)
**Sensitive data patterns for security testing**
- API key detection patterns
- Credit card format validation
- Email address patterns
- IP address discovery
- SSN format matching
- Phone number patterns

### Payloads (`security-payloads`)
**Specialized attack payloads for testing**
- XSS injection vectors
- XXE payloads
- Template injection
- File upload bypasses
- Path traversal strings

### Usernames (`security-usernames`)
**Common username wordlists**
- Default usernames
- Common account names
- Service-specific usernames
- Admin account patterns

### Web-Shells (`security-webshells`)
**Web shell samples for detection and analysis**
- PHP web shells
- ASP/ASPX shells
- JSP shells
- Python shells
- Perl shells

### LLM Testing (`llm-testing`)
**Comprehensive AI/ML security testing prompts**
- Bias detection (gender, nationality, race/ethnicity)
- Data leakage and privacy testing
- Memory recall testing
- Alignment and divergence attacks
- Adversarial prompt resistance
- AI safety evaluation

## Requirements

- **Node.js** (for `npx skills` — the skills.sh install CLI)
- A supported AI agent (Cursor, Claude Code, Codex, OpenCode, etc.)
- Git for cloning the repository
- Basic understanding of security testing concepts
- Authorization for security testing on target systems

## Installation

### Method 1: skills.sh CLI (Recommended)

Install skills into your agent using the [skills.sh](https://skills.sh/) ecosystem:

```bash
# See what's available
npx skills add Eyadkelleh/awesome-skills-security --list

# Install everything
npx skills add Eyadkelleh/awesome-skills-security --skill '*' -y

# Install to Cursor only
npx skills add Eyadkelleh/awesome-skills-security -a cursor --skill '*' -y

# Update installed skills later
npx skills update -y
```

Skills are installed to your agent's skills directory (e.g. `.cursor/skills/` for Cursor, `.claude/skills/` for Claude Code). Use `-g` for a global install available across all projects.

### Method 2: Clone Repository

Clone and use directly:

```bash
git clone https://github.com/Eyadkelleh/awesome-skills-security.git
cd awesome-skills-security
```

## Usage

### Using Skills in Natural Language

Reference skills in your conversation with any supported agent:

```
"Use the security-fuzzing skill to help me test for SQL injection vulnerabilities"

"Show me common passwords from the security-passwords skill"

"Help me detect exposed API keys using the security-patterns skill"

"I need XSS payloads from the security-payloads skill"
```

### Practical Usage Examples

**Example 1: SQL Injection Testing**
```
"I need to test a login form for SQL injection. Use the security-fuzzing skill to show me relevant payloads"
```

**Example 2: Password Auditing**
```
"Use the security-passwords skill to show me the most common weak passwords to test against our password policy"
```

**Example 3: Code Review for Secrets**
```
"Use the security-patterns skill to help me scan this codebase for exposed API keys and credentials"
```

**Example 4: CTF Challenge**
```
"I'm working on a web exploitation CTF challenge. Use the security-payloads skill to help me approach this"
```

**Example 5: LLM Security Testing**
```bash
# Test for AI model biases
"Use the llm-testing skill to help me test this AI model for gender bias"

# Check for data leakage vulnerabilities
"Use the llm-testing skill to test for data leakage and privacy issues in this LLM"

# Comprehensive AI safety audit
"I need to perform a red team assessment on this LLM. Use the llm-testing skill to show me prompts for bias detection, alignment testing, and adversarial resistance"
```

### Direct File Access

If you cloned the repository, access wordlists directly:

```python
# Example: Load SQL injection payloads
with open('skills/security-fuzzing/references/Fuzzing/quick-SQLi.txt', 'r') as f:
    sqli_payloads = f.read().splitlines()

# Example: Load common passwords
with open('skills/security-passwords/references/500-worst-passwords.txt', 'r') as f:
    passwords = f.read().splitlines()

# Example: Use in security testing
for payload in sqli_payloads[:10]:
    test_injection(target_url, payload)
```

### Example Workflows

**SQL Injection Testing (Authorized)**
```
1. Ask your agent to use the security-fuzzing skill
2. Request relevant payloads for your target database
3. Test in an authorized scope
4. Document all findings
```

**CTF Challenge**
```
1. Describe the challenge to your agent
2. Ask it to use security-payloads or security-fuzzing as needed
3. Access relevant wordlists from the skill references
```

**Bug Bounty Hunting**
```
1. Ask your agent to use the appropriate security skills for your target
2. Review scope and methodology
3. Use payloads and wordlists from the installed skills
4. Follow responsible disclosure practices
```

## Project Structure

```
awesome-skills-security/
├── README.md                                    # This file
└── skills/                                      # skills.sh compatible skill directories
    ├── security-fuzzing/
    │   ├── SKILL.md                            # Skill metadata
    │   └── references/                         # SQL/NoSQL/Command injection
    ├── security-passwords/
    │   ├── SKILL.md
    │   └── references/                         # Password wordlists
    ├── security-patterns/
    │   ├── SKILL.md
    │   └── references/                         # API keys, sensitive data
    ├── security-payloads/
    │   ├── SKILL.md
    │   └── references/                         # XSS, XXE, file upload
    ├── security-usernames/
    │   ├── SKILL.md
    │   └── references/                         # Username wordlists
    ├── security-webshells/
    │   ├── SKILL.md
    │   └── references/                         # Web shell samples
    └── llm-testing/
        ├── SKILL.md
        └── ...                                   # LLM security test prompts
```

## Features

- **7 Skill Categories** - Fuzzing, Passwords, Patterns, Payloads, Usernames, Web-shells, LLM Testing
- **Curated from SecLists** - Essential security testing wordlists and payloads
- **AI/ML Security Testing** - Comprehensive LLM testing prompts for bias, alignment, and safety
- **Multi-Agent Support** - Install via skills.sh into Cursor, Claude Code, Codex, and 60+ agents
- **Ethical Guidelines** - Built-in reminders for authorized use only

## Security & Ethics

### Authorized Use Cases

- Authorized penetration testing with written permission
- Bug bounty programs (within documented scope)
- CTF competitions and challenges
- Security research in controlled lab environments
- Testing your own systems and applications
- Educational demonstrations with proper safeguards
- Defensive security tool development
- AI/ML security research and red team operations
- LLM safety evaluation and bias testing
- Responsible AI development and testing

### Prohibited Use Cases

- Unauthorized access attempts against any system
- Testing systems without explicit permission
- Malicious activities or attacks
- Privacy violations or data theft
- Any illegal activities
- Attacks against critical infrastructure
- Mass exploitation or automated attacks

### Responsible Usage Guidelines

1. **Always obtain written authorization** before conducting security tests
2. **Stay within scope** of authorized testing boundaries
3. **Document all activities** during security assessments
4. **Report vulnerabilities responsibly** through proper disclosure channels
5. **Respect rate limits** and avoid denial-of-service conditions
6. **Protect sensitive data** discovered during testing
7. **Follow applicable laws** and regulations in your jurisdiction

## Why This Project Exists

SecLists is an incredible resource containing over 6,000 files and 4.5GB of security testing data. However, its size and breadth can be overwhelming. This project:

- **Curates essential lists** most commonly needed for security testing
- **Organizes by category** for easy discovery and access
- **Integrates with AI agents** via the skills.sh ecosystem for seamless workflow integration
- **Provides clear documentation** on when and how to use each resource
- **Emphasizes ethical use** with clear guidelines and warnings

## Source & Attribution

All security testing resources in this repository are sourced from [SecLists](https://github.com/danielmiessler/SecLists) by Daniel Miessler and contributors.

- **Original Repository:** https://github.com/danielmiessler/SecLists
- **License:** MIT License
- **Maintainer:** Daniel Miessler
- **Contributors:** Security community worldwide

This project is a curated, skill-packaged subset for agent skill integration. For the complete SecLists collection (4.5GB, 6,000+ files), visit the original repository.

## Best Practices

### When Using Password Lists
- Only test against systems you own or have written authorization to test
- Implement rate limiting to avoid account lockouts
- Monitor for defensive responses (WAF blocks, account locks)
- Use appropriate delays between attempts

### When Using Fuzzing Payloads
- Test in isolated environments first
- Validate input sanitization and output encoding
- Check for secondary effects (logs, monitoring alerts)
- Document all findings systematically

### When Using Web Shells
- Only use for detection system validation
- Test in isolated lab environments
- Never deploy on production systems
- Focus on defensive detection capabilities

## Contributing

Contributions are welcome! If you'd like to:

- Add new curated wordlists
- Improve documentation
- Fix errors or update outdated information
- Suggest additional skills

Please open an issue or pull request.

## How to Use This on skills.sh

This repository is published on the [skills.sh](https://skills.sh/) open agent skills directory — the public registry for the [Agent Skills](https://agentskills.io) ecosystem. Skills are discovered from the `skills/` directory and appear on the [skills.sh leaderboard](https://skills.sh/) as users install them.

**Collection page:** [skills.sh/Eyadkelleh/awesome-skills-security](https://skills.sh/Eyadkelleh/awesome-skills-security)

### What is skills.sh?

[skills.sh](https://skills.sh/) is the directory and CLI for reusable agent skills. A single install command works across Claude Code, Cursor, Codex, OpenCode, and dozens of other agents. No separate packaging or publish step is required — push valid `SKILL.md` files to a public GitHub repo and users can install immediately.

### For Users

```bash
# Browse what's available
npx skills add Eyadkelleh/awesome-skills-security --list

# Install all skills (project scope)
npx skills add Eyadkelleh/awesome-skills-security --skill '*' -y

# Install one skill to Cursor
npx skills add Eyadkelleh/awesome-skills-security --skill security-fuzzing -a cursor -y

# Search the skills.sh directory
npx skills find security
```

After installing, ask your agent to use a skill naturally:

```
"Use the security-fuzzing skill to show me SQL injection payloads"
```

### Supported Agents

Install to any supported agent with the `-a` flag:

| Agent | Install example |
|:------|:----------------|
| Cursor | `npx skills add Eyadkelleh/awesome-skills-security -a cursor -y` |
| Claude Code | `npx skills add Eyadkelleh/awesome-skills-security -a claude-code -y` |
| Codex | `npx skills add Eyadkelleh/awesome-skills-security -a codex -y` |
| OpenCode | `npx skills add Eyadkelleh/awesome-skills-security -a opencode -y` |

See the full list of [supported agents](https://skills.sh/).

### SKILL.md Requirements

Each skill directory must contain a `SKILL.md` with YAML frontmatter:

```yaml
---
name: security-fuzzing
description: "Essential fuzzing payloads: SQL injection, command injection, and more."
---
```

- `name` — lowercase identifier with hyphens only (e.g. `security-fuzzing`)
- `description` — non-empty; quote values that contain colons

### For Contributors

Want to add your own skills to this collection?

1. **Fork this repository**
2. **Add your skill** under `skills/your-skill-name/`
3. **Create a SKILL.md** with valid frontmatter (`name` must be lowercase with hyphens, plus `description`)
4. **Verify locally**: `npx skills add . --list`
5. **Submit a pull request** with a description of your contribution

### Publishing Your Own Skills

To create your own skill collection for skills.sh:

1. **Create a repository** with a `skills/` directory
2. **Add SKILL.md files** in each skill directory with `name` and `description` frontmatter
3. **Push to GitHub** and make it public
4. **Verify discovery**: `npx skills add username/repo-name --list`
5. **Share your repo** — users install with `npx skills add username/repo-name`

## Related OSINT Tools

| Tool | Description |
|:-----|:------------|
| [x-twitter-scraper](https://github.com/Xquik-dev/x-twitter-scraper) | X/Twitter OSINT skill — user lookup, follower extraction, engagement analysis, account monitoring. MCP server, REST API, 20 extraction tools. |

## Documentation and References

- [skills.sh Directory](https://skills.sh/) - Browse and install agent skills
- [This collection on skills.sh](https://skills.sh/Eyadkelleh/awesome-skills-security) - Install stats and skill listing
- [Agent Skills Specification](https://agentskills.io) - SKILL.md format and conventions
- [skills CLI (npm)](https://www.npmjs.com/package/skills) - `npx skills` install and manage skills
- [Cursor Skills Documentation](https://cursor.com/docs/context/skills) - Using skills in Cursor
- [Claude Code Skills Documentation](https://code.claude.com/docs/en/skills) - Using skills in Claude Code
- [SecLists Official Repository](https://github.com/danielmiessler/SecLists)
- [OWASP Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [Bug Bounty Platforms](https://github.com/disclose/bug-bounty-platforms)
- [Responsible Disclosure Guidelines](https://cheatsheetseries.owasp.org/cheatsheets/Vulnerability_Disclosure_Cheat_Sheet.html)

## License

MIT License - Use responsibly with proper authorization.

This is a curated collection and redistribution of SecLists content. The original SecLists project is maintained by Daniel Miessler under the MIT License. All credit for the original content goes to the SecLists project and its contributors.

## Disclaimer

This repository is provided for educational and authorized security testing purposes only. The maintainers of this repository are not responsible for any misuse or damage caused by the resources contained herein. Users are solely responsible for ensuring they have proper authorization before conducting any security testing activities.

---

**Note:** This is a curated reference repository. Always verify you have proper authorization before conducting security testing. When in doubt, ask for explicit written permission.

**Awesome Security Skills** | Security Collection for [skills.sh](https://skills.sh/)
