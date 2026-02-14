# AGET Reviewer Template

> **Quality assurance and review template**

Part of the [AGET Framework](https://github.com/aget-framework) v3.5.0.

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

---

## Specification

| Attribute | Value |
|-----------|-------|
| **Governed By** | [AGET_TEMPLATE_SPEC v3.1](https://github.com/aget-framework/aget/blob/main/specs/AGET_TEMPLATE_SPEC.md) |
| **Foundation** | [WORKER_TEMPLATE_SPEC v1.0](https://github.com/aget-framework/aget/blob/main/specs/WORKER_TEMPLATE_SPEC_v1.0.yaml) |
| **Archetype** | Reviewer |
| **Extends** | Consultant |
| **Manifest Version** | 3.0 |
| **Contract Tests** | 8 tests |

### Key Capabilities

| ID | Capability | Pattern |
|----|------------|---------|
| CAP-001 | Wake Protocol | event-driven |
| CAP-009 | Wind Down Protocol | event-driven |
| CAP-020 | Version Configuration | ubiquitous |
| CAP-028 | Project Plan Pattern | event-driven |

Validate compliance: `pytest tests/ -v`

See: [Full specification](https://github.com/aget-framework/aget/tree/main/specs)

---

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
