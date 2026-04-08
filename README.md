# CD Security — Claude Code Skills

A collection of [Claude Code](https://claude.ai/claude-code) skills built by [CD Security](https://cdsecurity.io) to help development teams ship safer smart contracts.

These skills automate the tedious parts of security preparation so teams can focus on building — and auditors can focus on finding real bugs instead of chasing missing documentation and untested code.

## Skills

| Skill | Language | Command | Description |
|-------|----------|---------|-------------|
| [audit-prep](audit-prep/) | Solidity | `/audit-prep` | 8-phase readiness check for Foundry & Hardhat projects |
| [rust-audit-prep](rust-audit-prep/) | Rust | `/rust-audit-prep` | 5-phase readiness check for Anchor & native Solana programs |

Each skill has its own README with detailed usage, phases, and options.

## Disclaimer

These tools are **not bug hunters**. They do not find vulnerabilities, detect complex bugs, or perform any form of security analysis. They are **not a substitute for a security audit**.

They check that your project's tests, documentation, code hygiene, and infrastructure are in order *before* an audit begins, so auditors can spend their time on what matters: finding real bugs.

## Prerequisites

- [Claude Code](https://claude.ai/claude-code) installed and authenticated

## Install

Clone the repo and symlink the skills you want into your Claude Code skills directory:

```bash
git clone https://github.com/CDSecurity/cdsecurity-skills.git ~/cdsecurity-skills
```

**Solidity projects:**
```bash
ln -s ~/cdsecurity-skills/audit-prep ~/.claude/skills/audit-prep
```

**Rust/Solana projects:**
```bash
ln -s ~/cdsecurity-skills/rust-audit-prep ~/.claude/skills/rust-audit-prep
```

To update later:

```bash
cd ~/cdsecurity-skills && git pull
```

## Contributing

Found a bug? Have an idea for a new check? PRs and issues are welcome.

If you build a skill that helps make smart contracts safer, we'd love to include it.

## License

[MIT](LICENSE) © CD Security

## About CD Security

[CD Security](https://cdsecurity.io) is a smart contract security firm. We perform manual security audits, build security tooling, and contribute to making the ecosystem safer for everyone.
