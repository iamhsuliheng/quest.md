# RATIONALE.md

The reasoning behind QUEST.md's design.

---

## The Problem

Most project documents are structured as plans. They describe what
will be done, by when, and by whom. They are useful for coordination.
They are less useful for navigation.

A plan assumes that the destination is settled, the route is known,
and the primary work is execution. This assumption breaks quickly.
In practice, the destination shifts as you learn more. The route
changes as reality pushes back. The original reason the project
existed can be forgotten entirely as tactical pressures accumulate.

A project document that only holds a plan has no way to record these
changes, and no way to help the people doing the work stay oriented
when the plan no longer matches the situation.

QUEST.md is designed for projects that require navigation, not just
execution: undertakings where the destination is real but not yet
fully known, where the route will change, and where the meaning of
the work matters as much as the steps.

---

## The Framework

QUEST.md is built on a cybernetics feedback loop.

In cybernetics, a system maintains direction through three elements:
a reference state (where you want to be), a measured state (where
you are), and a control action (what you do to close the gap). The
system does not execute a fixed plan — it continuously compares
where it is to where it wants to be, and adjusts.

In QUEST.md, these map to:

- **Destination** — the reference state: where you want to arrive
- **Current Situation** — the measured state: where you are now
- **Route** — the control action: what you are doing to close the gap

What cybernetics adds to ordinary project thinking is the recognition
that both the reference state and the measured state are models, not
facts. Your picture of the destination is an imagination. Your reading
of the current situation is an interpretation. Both can be wrong, and
both are expected to change.

This is why Route is described as an imagination, not a plan. Route
is your best current thinking about how to get from here to there.
It is held under pressure from reality. The Journal records how it
changes over time.

---

## Design Decisions

### Why "Quest," not "Project"

"Project" carries a strong association with deliverables, timelines,
and resource allocation — the vocabulary of execution. "Quest"
carries an association with a journey whose destination matters and
whose path is not fully known.

The choice is deliberate. QUEST.md is designed for undertakings
where meaning and navigation matter, not just delivery. The name
signals that orientation.

QUEST.md is also designed as a companion to CHARACTER.md. Both
documents model something that lives and changes over time — a
character, a journey — rather than something that is built once and
deployed.

### Why two layers: strategic and tactical

Most project documents go directly to the tactical: what are we
doing, how are we doing it, who is doing it. This is efficient when
the reason for the work is obvious. It becomes a liability when the
reason is contested, unclear, or at risk of being forgotten.

The strategic layer — Crisis and Resolution — exists to hold that
reason explicitly. It answers a different question than the tactical
layer: not "where are we going and how," but "why does this quest
exist and what kind of response are we making." Establishing the
strategic layer first ensures that tactical decisions can be
evaluated against it.

### Why "Crisis" and "Resolution," not "Problem" and "Goal"

"Problem" implies a puzzle with a correct solution. "Crisis" implies
a situation that has broken normal conditions and requires a
response. Crisis is a better description of why most meaningful
work begins: something changed, something broke, something can no
longer continue as before.

"Resolution" is not the solution to the Crisis and not the
destination of the journey. It is the strategic orientation chosen
in response. It describes what kind of response this quest
represents — the direction, not the arrival point. Using "Solution"
would suggest the Crisis has been answered; Resolution preserves the
tension that makes the journey necessary.

### Why Resolution includes "why not the most obvious alternatives"

A direction only becomes legible when you understand what was
considered and set aside. The most common alternatives to any
strategic choice are the ones readers will think of first. If those
alternatives are not addressed, readers who would have chosen
differently cannot understand why this direction was chosen —
and cannot meaningfully evaluate whether the quest is still
on track.

This is borrowed from Architecture Decision Records (ADR), which
include an "alternatives considered" section for exactly this reason.

### Why Destination does not require measurability

The standard advice for goals — make them specific and measurable —
is designed to ensure accountability and to avoid vague commitments.
It is useful for tasks. It is less useful for destinations.

A destination is the imaginable scene of completion. The test for a
good Destination is not whether it can be quantified, but whether
the people working toward it can picture it clearly enough to
recognize when they have arrived. Many worthwhile destinations
cannot be measured but can be imagined: a relationship repaired,
a community established, a work completed.

Requiring measurability would exclude exactly these destinations.
Requiring imaginability preserves what measurability is trying to
achieve — clarity and recognizability — without imposing a
constraint that does not fit the territory.

### Why Status is a single line at the top

A document's lifecycle state — whether the quest is active,
completed, or abandoned — is the first thing a reader needs to know.
It changes how every other section is read.

Status is placed at the top, before any content, so that a reader
who encounters a QUEST.md for the first time can orient immediately.
Three values cover the territory: the quest is in progress, it
reached its destination, or it ended before it did. "Abandoned" is
distinguished from "completed" because the reason a quest ends
matters — a quest that reached its destination tells a different
story than one that did not.

### Why Takeaways comes before Entries in the Journal

The Journal has two parts. Takeaways is a distillation: what the
quest has taught you, written as understanding rather than log.
Entries is a chronological record of what changed and when.

Takeaways is placed first because it is the part most likely to be
useful on re-reading. When you return to a Journal to understand
where a quest has been, the distillation is more valuable than the
log. Entries grows append-only over time; Takeaways is the
interpretation of that growth.

---

## Relation to CHARACTER.md

QUEST.md is designed as a companion specification to CHARACTER.md.

CHARACTER.md defines a format for describing a character: who
someone is, what they know, and what they have experienced.
QUEST.md defines a format for describing an undertaking: why it
exists, where it is going, and how the journey has moved.

Both specifications describe something that lives and changes over
time. Both use the Journal as the mechanism for recording that
change. Both prioritize semantic structure over document format.

A CHARACTER.md and a QUEST.md can be used together: the character
pursues the quest, and both documents grow as the work proceeds.
