# Contributing to Awesome Agent Trace

Thanks for helping build the map of agent-trace research! 🙌

## Scope

We collect papers, benchmarks, datasets, standards, and tools that **record, represent, attribute, inspect, constrain, diagnose, repair, or learn from agent execution traces**. This includes:

- Trace representation, provenance models, schemas, and standards
- Evidence attribution and grounding (claim–evidence support)
- Error/failure taxonomies and failure attribution / trace debugging
- Runtime provenance: injection defense, information-flow control, guardrails
- Memory provenance, memory poisoning/defense, long-term audit
- Learning from traces: experience/skill libraries, trajectory distillation, process rewards, credit assignment
- Observability platforms, debuggers, and analysis tooling
- Benchmarks and datasets with trace-level annotations

Out of scope: general agent papers without a trace/provenance angle, pure prompt-engineering tips, and non-agent LLM applications.

## Entry Format

Follow the existing numbered template:

```markdown
N. **Paper Title** (Venue Year)

   *First Author, Second Author, et al.*

   [[Paper]](https://arxiv.org/abs/XXXX.XXXXX) [[Code]](https://github.com/org/repo) -- One-line note on what it does and why it matters for agent traces.
```

Rules:

- Keep numbering **sequential** within the whole document (do not restart per section).
- Place the entry in the correct category and subsection; update the TOC anchor if you add a new section.
- Verify links before submitting: arXiv IDs must resolve; GitHub repos must return 200.
- Prefer arXiv links for papers; add `[[Code]]` / `[[Data]]` links when an official artifact exists.
- One-line notes should say *what the work does*, not generic praise.
- Benchmarks and datasets with trace annotations should also be added to the **Benchmarks & Datasets** table (name, link, scale, annotation granularity).
- If a paper has been retracted or withdrawn, do not add it; if it is already listed, add a ⚠️ note (see GraphTracer).

## Pull Requests

1. Fork → branch (`add-xxx`) → commit → PR.
2. Use a descriptive PR title, e.g. `Add FALAT (hierarchical dependency-guided failure attribution)`.
3. New category proposals are welcome, but please open an issue first to discuss placement.

## Reporting Issues

Found a dead link, wrong venue, or a misclassified paper? Please open an issue with the entry number.
