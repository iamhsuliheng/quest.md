Status: active

# QUEST.md

## Crisis

Project documentation has two failure modes. The first is
mechanism-based tooling — tickets, boards, milestones, Gantt
charts — that tracks activity without capturing intent. The second
is free-form notes that capture intent without giving it structure.
Neither answers the question a collaborator actually needs answered
when joining a project: why does this exist, where is it going, and
what is blocking it right now.

The gap became visible while building CHARACTER.md. A character
document — something most people would call "just a system prompt"
— turned out to benefit from a semantic specification: three
sentence types, each with a distinct function, all in plain text.
If that was true for character documents, it should be true for
project documents too.

## Resolution

Build an open semantic specification for project documents that
defines what sentences mean, not how documents look.
Medium-agnostic, plain text, no tooling required. Read SPEC.md to
understand the structure, then create a QUEST.md in your project.

This direction over alternatives: a format-prescriptive approach
(like Amazon's 6-pager) would impose page limits and prose style,
making it too heavy for individual or small-team use. A
tooling-based approach (like ADRs in CI pipelines) would exclude
anyone not working in a software repository. A semantic spec that
defines meaning without dictating structure stays portable and
accessible to the widest range of undertakings.

---

## Destination

QUEST.md is a named format. Developers and writers reach for it
the way they reach for README.md — not because a tool requires it,
but because the format does useful work and they know what it means.
The spec is stable enough that tools can be built on top of it and
people can teach it.

The scene: someone new to a project opens QUEST.md and immediately
understands why the project exists, where it is going, and what is
in the way. No onboarding conversation needed.

## Current Situation

The spec exists. SPEC.md and README.md are published at
github.com/iamhsuliheng/quest.md. The structure is defined and
internally consistent. This QUEST.md is the first filled example.

What is still missing: examples from other domains. A single
self-describing example shows the format works but does not show
how it generalizes. A reader working on a writing project, an
event, or a product launch cannot yet see themselves in an example.
That is what is blocking broader adoption.

## Route

Add at least one example from a different domain — a writing
project, an event, a product launch — so readers can generalize
the format beyond the spec itself.

Cross-promotion alongside character.md is already in place via the
See also link. No additional distribution work needed at this stage.

## Fellowship

**iamhsuliheng** — spec author and maintainer.

**character.md** — companion spec. Proved the model: a semantic
specification for a plain-text format can be stable, portable, and
useful without tooling. QUEST.md describes what a character is
doing. character.md describes who that character is.

**The four gods** — co-designed the two-layer structure, the
decision to extract Journal as a standalone element, and the
removal of the Sentence types section.

## Journal

### Takeaways

- A semantic spec needs at least one filled example to be
  believable; self-describing examples are immediately verifiable.
- Status, Resolution alternatives, and Journal structure are the
  three things most project document formats get wrong by omission.
- Defining meaning without prescribing format keeps a spec portable
  across domains and team sizes.

### Entries

2026-06-25 — Added Status line, expanded Resolution to include
alternatives considered, split Journal into Takeaways and Entries.

2026-06-25 — README Getting started rewritten. Removed instruction
to copy SPEC.md (a spec is not a template). Replaced with an
ordered list of sections and the note that Journal starts when
something first changes.

2026-06-25 — Initial spec published. Structure defined as two
layers (Strategic + Tactical) plus Journal as a standalone running
record. Sentence types section removed as redundant. QUEST.md
renamed SPEC.md to distinguish the spec from filled instances.
This QUEST.md added as the first self-describing example.
