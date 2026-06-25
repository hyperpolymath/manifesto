<!--
SPDX-License-Identifier: CC-BY-SA-4.0
SPDX-FileCopyrightText: 2025-2026 Jonathan D.A. Jewell <j.d.a.jewell@open.ac.uk>
-->

<div class="lead" wrapper="1">

A turn from writing code to writing the rules, checks, and values that
code must answer to — and making all three legible enough to be
contested.

</div>

# The vision

For most of three decades I have worked across cognitive science,
philosophy, and systems engineering, mostly in private. This manifesto
marks the move into public: the deployment of the RSR 2026 (Rhodium
Standard Repository) and the body of work that surrounds it.

The thesis is simple to state and hard to live up to. Most of what
governs software is left implicit — intent lives in prose, soundness
lives in trust, value lives in authority. **The metaprogramming turn is
the decision to make those governing things explicit, first-class, and
inspectable**: to write not only the program, but the rules it must
obey, the checks that establish it, and the values it encodes, in a form
that both a machine and a critic can read and argue with.

I can begin this. I cannot finish it alone — and a manifesto about
making value contestable would contradict itself if it stayed a
monologue. So from here it is *we*.

We value, in the precise sense that this whole project is *about* value:

- explicit, contestable structure over implicit good faith;

- checked certainty over fluent plausibility;

- rigour applied wherever a problem demands it over rigour rationed to
  the problems we have agreed to call "technical".

# Core pillars

Each pillar is a position, not a slogan. Each is meant to be disagreed
with.

## 1. Machine-readable governance

The rules an estate lives by — licensing, provenance, conventions, who
may change what — should be encoded as machine-readable artifacts, not
narrated in prose that quietly drifts from the code it describes. A
human-centric README cannot be checked; governance-as-data can. The
`6SCM` pattern is how this estate encodes those rules so that tooling,
and AI agents, can verify conformance and flag drift rather than take a
paragraph’s word for it.

*What this rejects:* the prose README as the source of truth about how a
system is meant to behave.

## 2. Neurosymbolic verification

Probabilistic generation may propose; only symbolic method may dispose.
Where correctness matters, an unproven output from a language model is a
hypothesis, not a result, and treating fluency as evidence is a category
error. The discipline is to pair generation with mechanised checking so
that the part which can be certain has the last word.

*What this rejects:* plausibility mistaken for proof. (`hypatia` is the
clearest concrete instance.)

## 3. Post-disciplinary praxis

The rigour we reserve for compilers belongs equally to consent, to
policy, to accountability. The line between a "technical" problem that
deserves formal treatment and a "social" one left to good faith is
itself a choice — and often an alibi. Post-disciplinary means reaching
for whatever discipline the problem needs; *praxis* means refusing to
separate the theory from the practice that tests it. The same instinct
runs from labour-union policy to RISC-V SSGs.

*What this rejects:* the division of labour that keeps rigour out of the
rooms where power actually operates. (`avow-protocol`, consent-as-code,
is the most developed example.)

# The wager: value made legible

Underneath all three pillars is one bet. Deciding what a system *should*
do, whether an output *counts* as correct, who *consented*, and what
*matters* are all judgments of value — and they are usually smuggled in
implicitly and backed by authority: *trust me*, *the spec says so*, *the
model said so*. Axiology is the study of value; the metaprogramming turn
applies it operationally. Value is not asserted, it is *structured* —
and structure can be inspected, checked, and argued with.

This is also why the work is, at root, political as well as technical. A
value that is explicit and inspectable can be contested by the people it
bears on; a value backed only by authority cannot. Making value legible
is therefore a precondition for accountability — in a compiler, in an AI
system, and in a union. It is the point at which formal methods and
solidarity economics turn out to want the same thing: that the rules be
legible, and the powerful be answerable to them.

It is the same instinct that runs through the technical research —
identity defined by equivalence rather than asserted, a value justified
by the construction that produced it rather than taken on faith. The
manifesto only generalises that instinct, from values inside a program
to values inside our systems and institutions.

# Reading order

- `EXPLAINME.adoc` — the canonical "what is this" entry-point, consumed
  by AI agents and by the `hyperpolymath/standards` governance tooling.

- `docs/` — supporting essays, position papers, and ADRs that situate
  the manifesto in context.

- `MAINTAINERS.adoc` — current stewards.

# Status

- **Licence:** MPL-2.0 (migrated from PMPL-1.0-or-later on 2026-05-26
  per the estate licence-debt audit,
  [hyperpolymath/standards#196](https://github.com/hyperpolymath/standards/pull/196)).

- **Maturity:** a work in progress; the manifesto is a living document.
  The version number on the title line is incremented on each
  substantive revision.

- **Audit findings:** see `docs/tech-debt-2026-05-26.md` if present
  (added by the 2026-05-26 estate tech-debt scan).

# Engaging with this manifesto

Collaboration here is not decoration; by the argument above it is
constitutive. A manifesto that makes value contestable earns its keep
only by being contested, adopted, and extended. Three ways in:

- **Disagree** — open an Issue. Manifestos thrive on being argued with,
  and a pillar that no one challenges has not yet been tested.

- **Adopt a thread** — fork, riff, cite. The MPL-2.0 licence makes
  derivative manifestos easy.

- **Contribute editorially** — see
  <a href="CONTRIBUTING.md" class="md">CONTRIBUTING</a> for the
  (intentionally light) editorial conventions.

Whether you are a researcher, a maintainer, a journalist, or a student,
the door is open — and the NUJ and solidarity-economics threads here
mean I take "we" literally.

# Companion repositories

- `hyperpolymath/standards` — the RSR 2026 standards that the first
  pillar references.

- `hyperpolymath/hypatia` — the neurosymbolic analyser that is the
  second pillar’s clearest concrete instantiation.

- `hyperpolymath/avow-protocol` — the consent-as-code stack that is the
  third pillar’s most-developed example.
