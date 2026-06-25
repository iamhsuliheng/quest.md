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
document — something most people would call “just a system prompt”
— turned out to benefit from a semantic specification: three
sentence types, each with a distinct function, all in plain text.
If that was true for character documents, it should be true for
project documents too.

## Resolution

Build an open semantic specification for project documents that
defines what sentences mean, not how documents look.
Medium-agnostic, plain text, no tooling required. The spec should
be forkable: copy SPEC.md, rename it QUEST.md, fill it in.

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
internally consistent.

What is missing: examples. Without a filled-in QUEST.md to look
at, a new reader has no way to verify that the spec produces useful
documents. This is the same gap character.md had before examples/
was added. It is what is blocking adoption.

## Route

Add at least one example from a different domain — a writing
project, an event, a product launch — so readers can generalize
the format beyond the spec itself.

This QUEST.md is the first example. A self-describing example has
the advantage of being immediately verifiable: anyone reading the
spec can check whether the example is accurate.

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

2026-06-25 — Initial spec published. Structure defined as two
layers (Strategic + Tactical) plus Journal as a standalone running
record. Sentence types section removed as redundant. QUEST.md
renamed SPEC.md to distinguish the template from filled instances.
This QUEST.md added as the first self-describing example.
