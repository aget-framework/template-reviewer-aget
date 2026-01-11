# Reviewer Domain Vocabulary

**Version**: 1.0.0
**Status**: Active
**Owner**: template-reviewer-aget
**Created**: 2026-01-10
**Scope**: Template vocabulary (DRIVES instance behavior per L481)
**Archetype**: Reviewer

---

## Meta

```yaml
vocabulary:
  meta:
    domain: "review"
    version: "1.0.0"
    owner: "template-reviewer-aget"
    created: "2026-01-10"
    theoretical_basis:
      - "L481: Ontology-Driven Agent Creation"
      - "L482: Executable Ontology - SKOS+EARS Grounding"
    archetype: "Reviewer"
```

---

## Concept Scheme

```yaml
Reviewer_Vocabulary:
  skos:prefLabel: "Reviewer Vocabulary"
  skos:definition: "Vocabulary for reviewer domain agents"
  skos:hasTopConcept:
    - Reviewer_Core_Concepts
  rdf:type: skos:ConceptScheme
```

---

## Core Concepts

### Artifact

```yaml
Artifact:
  skos:prefLabel: "Artifact"
  skos:definition: "Work product subject to review"
  skos:broader: Reviewer_Core_Concepts
  skos:inScheme: Reviewer_Vocabulary
```

### Criteria

```yaml
Criteria:
  skos:prefLabel: "Criteria"
  skos:definition: "Standards against which artifacts are evaluated"
  skos:broader: Reviewer_Core_Concepts
  skos:inScheme: Reviewer_Vocabulary
```

### Finding

```yaml
Finding:
  skos:prefLabel: "Finding"
  skos:definition: "Issue or observation identified during review"
  skos:broader: Reviewer_Core_Concepts
  skos:inScheme: Reviewer_Vocabulary
```

### Severity

```yaml
Severity:
  skos:prefLabel: "Severity"
  skos:definition: "Impact level of a finding"
  skos:broader: Reviewer_Core_Concepts
  skos:inScheme: Reviewer_Vocabulary
```

### Recommendation

```yaml
Recommendation:
  skos:prefLabel: "Recommendation"
  skos:definition: "Suggested action based on findings"
  skos:broader: Reviewer_Core_Concepts
  skos:inScheme: Reviewer_Vocabulary
```

---

## Extension Points

Instances extending this template vocabulary should:
1. Add domain-specific terms under appropriate broader concepts
2. Maintain SKOS compliance (prefLabel, definition, broader/narrower)
3. Reference foundation L-docs where applicable
4. Use `research_status` for terms under investigation

---

## References

- L481: Ontology-Driven Agent Creation
- L482: Executable Ontology - SKOS+EARS Grounding
- R-REL-015: Template Ontology Conformance
- AGET_VOCABULARY_SPEC.md

---

*Reviewer_VOCABULARY.md v1.0.0 — SKOS-compliant template vocabulary*
*Generated: 2026-01-10*
