# PV-PP AI Decision Architecture White Paper Series

This repository contains a four-paper series on AI decision architecture
within the **Productive Value-Productive Power (PV-PP) framework**.

The series is written for program managers, business owners,
decision-system architects, and technically interested readers
responsible for decisions that AI agents are increasingly being asked to
make. It begins with familiar rules, thresholds, utility functions, and
weighted scoring, then asks a more fundamental question: **when is one
number an adequate representation of a decision, and when does the
decision require a richer architecture?**

The papers are intended to be read in order, but each can also stand on
its own.

## The Series

### White Paper 1 --- How AI Agents Make Decisions

**From Simple Rules to Scoring Systems and Automated Judgment**

Introduces the decision problem. It explains how AI agents are assigned
decisions, how simple rules differ from judgment, and how judgment is
often translated into weighted scores and scalar aggregation. It also
identifies the modeling choices that program managers and business
owners implicitly approve when they accept an automated decision system.

**File:**
`PV-PP_White_Paper_1_How_AI_Agents_Make_Decisions_v0.7_Publication_Edition.docx`

### White Paper 2 --- When Is a Utility Function Not Enough?

**What You Don't Know About Scalar Aggregation Can Hurt You**

Examines when a one-number model faithfully represents the decision an
organization intended to delegate and when it preserves only the
appearance of correctness. It distinguishes winner reproduction, ranking
representation, and process fidelity, and examines thresholds, hard
constraints, hidden state, and information loss.

**File:**
`PV-PP_White_Paper_2_When_Is_a_Utility_Function_Not_Enough_v0.4_Publication_Draft.docx`

### White Paper 3 --- Before You Build the Utility Function

**A Practical Test for Easy, Hard, and Impossible Scalarization**

Provides an architecture-selection test to use before tuning weights. It
distinguishes easy scalarization, difficult scalarization, and cases
that are impossible on the proposed scalar route because required
information or structure has already been discarded. It then lays out
the legitimate alternatives: use a simple score, engineer a richer
scalar model, enrich the representation, or move to a structured
decision architecture.

**File:**
`PV-PP_White_Paper_3_Before_You_Build_the_Utility_Function_v0.3_Publication_Draft.docx`

### White Paper 4 --- How to Design a PV-PP Decision System

**From Business Rules to Structured Governance, Sidecar Control, and
Runtime Execution**

Moves from architecture selection to implementation. It describes a
bounded path from business requirements and source authority to
structured decision artifacts, testing, sidecar governance, replay, and
runtime-integrated execution. The current publication draft reflects the
frozen **PV-PP Runtime API v0.70 / Runtime Interface Freeze 1** and
distinguishes common runtime responsibilities from application-specific
persistence and integration.

**File:**
`PV-PP_White_Paper_4_How_to_Design_a_PV-PP_Decision_System_v0.3_Publication_Draft.docx`

## The Central Question

Scalar aggregation is not inherently wrong. A utility function, weighted
score, or other scalar decision rule can be exactly the right
architecture when the relevant decision can legitimately be represented
that way.

The problem begins when the score is asked to carry distinctions that
the decision itself requires to remain separate: hard constraints,
governing domains, state or history, recovery requirements,
non-interchangeable capacities, or information that has already been
omitted from the scalar route.

The series therefore treats scalarization as an **architecture choice
before it is a weight-tuning problem**.

PV-PP does not prohibit scalar scoring. It provides a broader structured
framework in which scalar comparison can be used where it is valid
without requiring one number to represent the entire decision.

## Current Project Status

The PV-PP framework is an active research and implementation program.
The **PV-PP Runtime API v0.70** has reached **Runtime Interface Freeze
1**, establishing a frozen common runtime interface supported by
regression testing, developer documentation, executable examples, and a
native reference application.

The scalar-boundary analysis discussed in this series is based on
completed internal technical work. It has **not yet received independent
external peer review**. Broader framework publication and controlled
release of proof materials remain ongoing.

## Related PV-PP Resources

-   **Main PV-PP project site:** https://amundsenlance.github.io/
-   **PV-PP Runtime API:**
    https://github.com/AmundsenLance/PV-PP-Runtime-API

## Suggested Reading Order

Start with White Paper 1 if you are new to automated decision
architecture. Papers 2 and 3 progressively sharpen the scalarization
question. White Paper 4 is the implementation-oriented paper and is most
useful after the architectural distinctions in the first three papers
are clear.

## Author

**Lance Amundsen**

Productive Value-Productive Power (PV-PP) framework research program

------------------------------------------------------------------------

*September 2026*
