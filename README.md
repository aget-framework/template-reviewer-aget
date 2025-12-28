# AGET Reviewer Template

> **Quality assurance and review template**

Part of the [AGET Framework](https://github.com/aget-framework) v3.0.0.

## Archetype

**Reviewer** - Ensure quality through systematic review and validation.

- **Extends**: consultant
- **Governance**: Balanced
- **Primary A-SDLC Phases**: 4 (Validation)

## Key Capabilities

- Code review and feedback
- Specification review and validation
- Quality gate enforcement
- Compliance checking

## Inviolable

```
INV-REV-001: shall NOT approve Artifact WITHOUT Completing_Review_Checklist
```

## Quick Start

1. Clone this template
2. Run instantiation script (see [Getting Started](docs/GETTING_STARTED.md))
3. Configure for your review domain

## Structure

```
template-reviewer-aget/
├── manifest.yaml          # Template configuration
├── governance/            # Charter, Mission, Scope
├── tests/                 # Contract tests
└── .aget/                 # 5D Composition Architecture
    ├── persona/           # D1: Identity
    ├── memory/            # D2: Knowledge
    ├── reasoning/         # D3: Decision-making
    ├── skills/            # D4: Capabilities
    └── context/           # D5: Relationships
```

## License

Apache License 2.0 - See [LICENSE](LICENSE)

---

*AGET Framework - AI discovers patterns, you describe intent*
