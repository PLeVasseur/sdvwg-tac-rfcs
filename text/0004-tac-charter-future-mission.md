- RFC Title: Future TAC Mission, Scope, and Responsibilities
- Submission Date: 2026-10-27
- RFC PR: https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/4
- Follow-on Actions: Propose the future operating model (planned) and formal charter amendments (planned) separately; identify willing preparers and required approvals

Status: Proposal for discussion; not adopted. Future RFC topics remain planned
and unsubmitted unless linked to an actual public proposal.

# Summary
[summary]: #summary

Propose an evidence-based technical stewardship mission for the Technical
Advisory Committee (TAC): help the Eclipse SDV Working Group develop a coherent,
credible open source ecosystem through purview recommendations, technical
ambition, lightweight architecture guidance, decision records, annual roadmap
signals, cross-project moderation, and specialist referrals. Guidance remains
non-mandatory, while the proposed TAC mandate includes making material
departures and their ecosystem implications transparent to the Steering
Committee. Projects and Project Management Committees (PMCs) retain project
governance and delivery. This RFC proposes future direction, not an amendment to the
[published Charter](https://www.eclipse.org/collaborations/working-groups/sdv/charter/).
It can be reviewed independently and in parallel with
[TAC New Way of Working — Markdown and GitHub (Draft PR #3)](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/3).

# Motivation
[motivation]: #motivation

Projects may meet their own objectives while leaving ecosystem questions
unanswered: how components fit together, which interfaces overlap, what a demo
demonstrates, or whose roadmap a dependency affects. The TAC needs an explicit
purpose and boundaries for turning those questions into useful recommendations,
without becoming a central implementation or project-management body.

The [current TAC duties](https://www.eclipse.org/collaborations/working-groups/sdv/charter/#technical-advisory-committee)
include purview recommendations, automotive and engineering policies, an annual
roadmap, coordinated releases, and integration work. This proposal retains the
purview anchor but deliberately proposes a different emphasis: technical
guidance, evidence, visibility, and referrals rather than TAC-owned release
orchestration and mandatory engineering policy. It does not claim that current
duties have already changed or that an existing process is inactive.

For example, two projects may choose different interfaces or runtimes for sound
local reasons. The proposed TAC role is to explain the resulting ecosystem
trade-off, invite project input, and identify a recommendation or referral—not
choose their implementation for them.

# Stakeholder impact
[stakeholder-impact]: #stakeholder-impact

In the proposed model, project contributors supply project-owned evidence and
can correct the TAC's interpretation. PMCs remain the project-governance path.
TAC participants prepare cross-project analysis; the Steering Committee receives
recommendations, material trade-offs, and questions requiring its action.
Specialist bodies receive topics within their own responsibilities.

An illustrative language/runtime orientation, such as C++14 or Rust for a
defined ecosystem objective, would explain its purpose and evidence rather than
mandate one stack. A project could choose differently. If that choice materially
affects a shared interface or integration activity, the TAC must record the
context, project response, and implications and make them visible to the
Steering Committee. The example selects no preferred language or version.

Similarly, a Blueprint integration opportunity becomes a discussion supported
by evidence, not an assigned project delivery commitment. Examples are
illustrative; no project participation or existing integration result is claimed.

# Detailed proposal
[detailed-proposal]: #detailed-proposal

## Proposed Mission

> Help the Eclipse SDV Working Group build a coherent, credible, and
> industry-relevant open source SDV ecosystem through transparent technical
> guidance, evidence-based purview recommendations, and cross-project insight.

## Responsibilities And Change From The Published Baseline

The comparison below uses the
[published TAC duties](https://www.eclipse.org/collaborations/working-groups/sdv/charter/#technical-advisory-committee),
not an assumed account of today's meeting practice. The future column is a
proposal; it does not supersede the Charter. Future content proposals remain
planned and unsubmitted; they are not adopted guidance.

| Responsibility | Proposed future direction | Relationship to the published baseline |
| --- | --- | --- |
| Project purview | Maintain transparent evidence criteria and explain recommendations to the Steering Committee. | Retain the recommendation duty; coordinate method details with [purview PR #2](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/2). |
| Technical ambition | Explain intended SDV fit through use cases, code-first evidence, demonstrability, engineering practice, and ecosystem roles. | Make the technical direction explicit as proposed non-mandatory guidance, not a new project implementation rule. |
| Architecture principles | Maintain lightweight principles for modularity, interface ownership, interoperability, and integration readiness. | Develop an advisory expression of architecture/integration work, coordinated with [reference-architecture PR #1](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/1), not a duplicate architecture specification. |
| Decision records | Preserve ecosystem questions, options, evidence, rationale, recommendations/referrals, status, and follow-up. | Add an explicit lightweight reasoning framework; link formal dispositions and project architecture decision records rather than replace them. |
| Material-deviation transparency | Report material departures from published ambition/principles, including context, evidence, project response, ecosystem implications, and follow-up. | Propose an explicit TAC reporting duty paired with non-mandatory guidance; do not claim this mandate already exists. |
| Roadmaps and releases | Review project-owned roadmap signals at least annually; surface dependencies, gaps, and integration opportunities. | Propose reframing the annual roadmap and coordinated-release duties toward ecosystem visibility. This requires formal consideration, not an informal waiver. |
| Engineering evidence and referrals | Share useful maturity, quality, safety, security, supply-chain, release, and demonstration evidence; refer specialist governance questions. | Propose reframing policy-enforcement duties toward advisory evidence handling. Applicable Foundation and specialist requirements remain in force. |
| Cross-project moderation | Convene affected projects/PMCs on overlaps, conflicting interfaces, integration opportunities, and unclear ownership. | Retain an integration concern while proposing recommendation/referral outputs rather than TAC control of project plans. |

## Authority And Boundaries

This proposed future model does not transfer code, roadmap, release, or
implementation ownership from projects and PMCs. Their governance remains
subject to the [Eclipse Foundation Development Process](https://www.eclipse.org/projects/dev_process/).
The TAC is not a project product owner, certification body, or replacement for
the Specification Committee, Functional Safety Committee, or Marketing and
Brand Committee described in the
[Working Group Charter](https://www.eclipse.org/collaborations/working-groups/sdv/charter/).

TAC guidance is non-mandatory; transparency is a duty of the TAC in the proposed
model, not a veto over project decisions. Materiality means a departure with a
credible ecosystem effect—for example on interoperability, a shared interface,
integration readiness, or Working Group strategy—not every local variation.
The subsequent decision-record proposal (planned)
should define practical examples and review
triggers. Projects must be able to provide their context before a recommendation.
Reporting is informational, not a project compliance finding.

The Steering Committee retains Working Group scope and strategy decisions.
Concrete distribution/release activities need their own appropriate mandate;
this proposal does not create a unified release train. Existing TAC obligations
remain effective until changed through the applicable governance route.

## Parallel Review And Separate Follow-On Work

This mission direction and
[TAC New Way of Working — Markdown and GitHub (Draft PR #3)](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/3) are independent
decisions that may be reviewed in parallel under the
[existing RFC process](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/README.md#what-the-process-is).
Neither needs the other to be accepted first. This mission can be considered
using current RFC and official-record arrangements; adopting a working medium
does not adopt this mission. If either proposal is deferred, the other can
still be considered on its own merits.

Develop the operating-model proposal (planned)
against the actual outcomes of both reviews: which
responsibilities are supported, which need further approval, how outputs are
prepared/reviewed, and where their records live. Mission detail belongs here;
record-location and routine-PR conventions do not. No new folders, scoring
thresholds, technical principles, or meeting cadence are adopted by this RFC.

Acceptance records the TAC's proposed direction, not a Charter amendment or
permission to stop current duties. Prepare
formal charter amendments (planned) separately
and identify the relevant approval route. Proposed principles for TAC
deliberation also require the applicable approvals identified in the
[TAC Charter section](https://www.eclipse.org/collaborations/working-groups/sdv/charter/#technical-advisory-committee).

Completion requires a recorded TAC position on the proposed responsibilities,
the changes requiring further approval, and the next operating-model/charter
actions. Identify willing preparers or leave assignments explicitly open;
acceptance does not invent owners or require adoption of the entire programme.

# Drawbacks
[drawbacks]: #drawbacks

The wider advisory scope could exceed available capacity. Guidance may be
mistaken for project mandates, and non-mandatory advice may not resolve an
integration conflict. Parallel reviews can drift apart. Keep their decisions
separate, reconcile them in the
operating model (planned), and prioritise work with
willing owners. Reframing existing duties also creates a transition that must
remain explicit until formal approvals are recorded.

# Rationale and alternatives
[rationale-and-alternatives]: #rationale-and-alternatives

Agreeing mission direction separately makes the purpose reviewable without
deciding every tool or technical criterion. Parallel review avoids holding that
discussion until routine-record arrangements are accepted. One combined
proposal would reduce cross-links but couple two different decisions. Keeping
the current duties unchanged is a legitimate alternative, but would not adopt
this proposed advisory emphasis. Central implementation control would conflict
with the intended project-ownership boundary.

# Prior art
[prior-art]: #prior-art

The [Working Group Charter](https://www.eclipse.org/collaborations/working-groups/sdv/charter/)
and [Development Process](https://www.eclipse.org/projects/dev_process/) establish
the governing baseline. This RFC proposes a direction within that context; it
does not infer authority from other communities' governance models.

Open [reference-architecture PR #1](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/1)
already proposes capability mapping and an end-to-end scenario; its
[review](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/1#pullrequestreview-5349473965)
raises integration with official project information. Open
[purview PR #2](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/2) already proposes
rating criteria and a sheet-based flow. This mission supplies neither a parallel
architecture nor another rating method, and determines neither PR's disposition.
Use the [published RFC process](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/README.md)
and [contribution rules](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/CONTRIBUTING.md)
for review rather than introduce another decision procedure.

# Unresolved questions
[unresolved-questions]: #unresolved-questions

- Before disposition: which responsibilities and boundaries does the TAC
  support, and which changes need
  Charter amendments (planned) or other approvals?
- Before implementation: which work has willing preparers and receiving bodies,
  and how should the transition preserve current duties while approvals remain
  pending? No participants or commitments are assigned by this draft.
- Follow-on: reconcile the independently reviewed
  [working-method outcome (Draft PR #3, pending review)](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/3) in the
  operating model (planned);
  develop ambition (planned),
  principles (planned),
  and decision records/materiality examples (planned)
  through their separately reviewed content proposals.

# Future possibilities
[future-possibilities]: #future-possibilities

Evaluate the resulting
operating model (planned)
through a small project-engagement pilot (planned)
with willing participants. Use real findings to adjust workload and reporting;
do not make a proposed pilot or a tool migration a prerequisite for discussing
the mission.
