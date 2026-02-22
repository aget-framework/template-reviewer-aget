# Template: Reviewer Agent

> Ensure quality through systematic artifact review and structured feedback

**Version**: v3.6.0 | **Archetype**: Reviewer | **Skills**: 2 specialized + 14 universal

---

## Why Reviewer?

The Reviewer archetype enforces **quality through systematic review**. Unlike casual feedback, reviewer agents provide:

- **Artifact review** — Evaluate documents, code, and designs against standards
- **Structured feedback** — Categorize findings by severity and actionability
- **Quality gates** — Ensure artifacts meet defined criteria before progression

**For evaluators**: If you need an AI that can review work products systematically and provide professional-grade feedback, the Reviewer archetype brings QA discipline to your workflow.

---

## Skills

Reviewer agents come with **2 archetype-specific skills** plus the universal AGET skills.

### Archetype Skills

| Skill | Description |
|-------|-------------|
| **aget-review-artifact** | Review artifacts against defined criteria. Produces structured assessment with pass/fail determinations. |
| **aget-provide-feedback** | Provide categorized feedback (blocking, suggestion, nitpick) with clear rationale and improvement paths. |

### Universal Skills

All AGET agents include session management, knowledge capture, and health monitoring:

- `aget-wake-up` / `aget-wind-down` — Session lifecycle
- `aget-create-project` / `aget-review-project` — Project management
- `aget-record-lesson` / `aget-capture-observation` — Learning capture
- `aget-check-health` / `aget-check-kb` / `aget-check-evolution` — Health monitoring
- `aget-propose-skill` / `aget-create-skill` — Skill development
- `aget-save-state` / `aget-file-issue` — State and issue management

---

## Ontology

Reviewer agents use a **formal vocabulary** of 6 concepts organized into 2 clusters:

| Cluster | Concepts |
|---------|----------|
| **Review Process** | Review, Artifact, Criteria |
| **Feedback** | Finding, Severity, Resolution |

This vocabulary enables precise communication about quality assurance.

See: [`ontology/ONTOLOGY_reviewer.yaml`](ontology/ONTOLOGY_reviewer.yaml)

---

## Quick Start

```bash
# 1. Clone the template
git clone https://github.com/aget-framework/template-reviewer-aget.git my-reviewer-agent
cd my-reviewer-agent

# 2. Configure identity
# Edit .aget/version.json:
#   "agent_name": "my-reviewer-agent"
#   "domain": "your-domain"

# 3. Verify setup
python3 -m pytest tests/ -v
# Expected: All tests passing
```

### Try the Skills

```bash
# In Claude Code CLI
/aget-review-artifact    # Review a document or code
/aget-provide-feedback   # Give structured feedback
```

---

## What Makes Reviewer Different

| Aspect | Casual Comments | Reviewer Agent |
|--------|----------------|----------------|
| **Review** | Informal opinions | Criteria-based assessment |
| **Feedback** | Mixed priorities | Categorized by severity |
| **Quality gates** | Subjective feel | Pass/fail determination |
| **Tracking** | Lost in conversation | Documented findings |

---

## Framework Specification

| Attribute | Value |
|-----------|-------|
| **Framework** | [AGET v3.6.0](https://github.com/aget-framework/aget) |
| **Archetype** | Reviewer |
| **Skills** | 16 total (2 archetype + 14 universal) |
| **Ontology** | 6 concepts, 2 clusters |
| **License** | Apache 2.0 |

---

## Learn More

- **[AGET Framework](https://github.com/aget-framework/aget)** — Core framework documentation
- **[Archetype Guide](https://github.com/aget-framework/aget/blob/main/docs/GETTING_STARTED.md)** — All 12 archetypes explained
- **[Getting Started](https://github.com/aget-framework/aget/blob/main/docs/GETTING_STARTED.md)** — Full onboarding guide

---

## Related Archetypes

| Archetype | Best For |
|-----------|----------|
| **[Developer](https://github.com/aget-framework/template-developer-aget)** | Code review (PR-specific) |
| **[Spec-Engineer](https://github.com/aget-framework/template-spec-engineer-aget)** | Requirements validation |
| **[Consultant](https://github.com/aget-framework/template-consultant-aget)** | Solution assessment |

---

**AGET Framework** | Apache 2.0 | [Issues](https://github.com/aget-framework/template-reviewer-aget/issues)
