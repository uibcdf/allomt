---
summary: Select the first bounded allostery workflow and specify its scientific contract.
issue: uibcdf/allomt#2
status: open
opened: 2026-11-15
closed:
verification: inspected
area: [scientific-design]
guard:
normative:
blocked_by: []
supersedes: []
---

# First scientific workflow

## What

Select one concrete biological question, representative input, method and useful
output before implementing AlloMT's first scientific operation. No numerical
method or broad result framework has been selected.

## How

Use [the scope](../SCIENTIFIC_SCOPE.md) to define applicable molecular identities,
selections and correspondence, states/frames, quantities, parameters, provenance,
uncertainty, negative/unsupported outcomes and interpretation limits. Inspect
existing provider APIs and place missing capabilities with their actual owners.

## Why

The prediction/characterization goal needs a method-specific, reproducible
scientific contract. A contact, score, correlation or elastic mode must retain
its actual meaning; source execution alone cannot establish a mechanism.

## Acceptance

- A first workflow, input and method are explicitly selected and documented.
- A minimal public operation and result contract fit that workflow.
- Provider reuse and any linked provider issues are concrete.
- A reproducible example and meaningful numerical/scientific checks include a
  negative or unsupported case and state their evidential limits.

Repository receiving remains uibcdf/allomt#1. This design issue can be discussed
while central membership remains pending in uibcdf/molsyssuite#202.
