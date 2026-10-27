- RFC Title: TAC New Way of Working — Markdown and GitHub
- Submission Date: 2026-10-27
- RFC PR: https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/3
- Follow-on Actions: Agree a small routine-record rollout and maintenance owners; consider the [advisory runway](#recommended-initial-pr-runway) separately

Status: Proposal for discussion; not adopted. Future RFC topics remain planned
and unsubmitted unless linked to an actual public proposal.

# Summary
[summary]: #summary

Adopt Markdown in [GitHub](https://github.com/PLeVasseur/sdvwg-tac-rfcs) as the
shared working medium for the Technical Advisory Committee's (TAC's) public
records: agendas, minutes, evidence, proposals, and follow-up. Keep these records
versioned, reviewed, and linked to their sources and outcomes. Routine records
use normal pull requests; substantial proposals use the
[published RFC process](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/README.md#when-you-need-to-follow-this-process).
Begin with a small maintained set of records and a non-binding recommended PR
runway toward the future TAC. This proposal does not change formal decision
authority or adopt the separately reviewed
[future mission (Draft PR #4)](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/4)
or charter amendments (planned).

# Motivation
[motivation]: #motivation

TAC participants need one discoverable route from a meeting or evidence source
to an action, proposal, or authoritative outcome. The
[repository README](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/README.md)
already defines how substantial proposals are developed and reviewed. This RFC
proposes the shared working medium and the home for routine public records,
without requiring every record to become an RFC.

For example, minutes should be easy to find and correct without writing a new
RFC. If those minutes describe a change to the
[purview method proposed in PR #2](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/2), they
should link the relevant RFC rather than become another copy of its policy.
This adds a home for routine records while retaining the established proposal
process and authoritative decision sources.

# Stakeholder impact
[stakeholder-impact]: #stakeholder-impact

The meeting-note author submits a dated Markdown file through a normal PR.
Reviewers correct the factual record and check action owners. The file has no
RFC number and does not use the nine-section
[RFC template](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/0000-template.md).
A participant proposing a substantial change follows the
[RFC process](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/README.md#what-the-process-is)
and links it from the minutes.

Projects can maintain their own evidence and plans, with TAC records linking
to them. Existing official minutes and formal decisions remain authoritative
under the [Working Group Charter](https://www.eclipse.org/collaborations/working-groups/sdv/charter/)
and applicable governing processes; the GitHub record links to those sources
instead of silently moving or duplicating them.

# Detailed proposal
[detailed-proposal]: #detailed-proposal

## Markdown Records And RFCs Serve Different Purposes

Apply the existing [RFC threshold](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/README.md#when-you-need-to-follow-this-process)
and [contribution process](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/CONTRIBUTING.md#contribution-process).
The examples below explain their application to the newly proposed routine
records; they do not introduce another review or decision procedure.

| Work item | Artifact and review route |
| --- | --- |
| Meeting agenda or factual minutes | Ordinary dated Markdown, reviewed through a normal PR; no RFC number/template. |
| Correction to minutes or update to an agreed action | Normal PR updating the record and linking any existing issue. |
| Factual evidence pack, clarification, or referral status under an agreed process | Ordinary Markdown with source links and status; any substantial new recommendation follows the existing RFC threshold. |
| Proposal to change TAC responsibilities, the purview method, or technical direction | RFC under the existing process; notes and evidence link to it. |
| Project-local code, roadmap, or architecture decision | Maintained by the project; linked from TAC work when relevant. |

Minutes can record a formal action and its authoritative source, but merging
minutes does not itself take that action. If a meeting proposes a substantial
change, record the discussion and link or prepare its RFC using the existing
process. A minor correction or routine record does not become a new RFC simply
because it is versioned in GitHub.

“Everything-as-code” means versioning the public working artifacts in scope,
not moving confidential material or project-owned originals into this
repository, and not turning every TAC activity into a proposal.

## Introduce Routine Records Incrementally

- Keep numbered RFCs in the [RFC directory](https://github.com/PLeVasseur/sdvwg-tac-rfcs/tree/main/text)
  (`text/`). Introduce routine records separately, initially
  proposing `meetings/YYYY-MM-DD.md` and a small `work/` area for evidence or
  follow-up summaries. Final paths are subject to maintainer agreement.
- Give each record the context it needs: minutes identify the meeting,
  discussion/outcomes, source links, and actions; an evidence pack identifies
  its topic, sources/date, status, and questions. Do not impose RFC metadata or
  a universal form on every record.
- Maintain one source for each fact, policy, or decision. Link accepted RFCs,
  official records, project-owned artifacts, and existing issues rather than
  create parallel policy text or a second task/decision log. A short navigation
  index shows what exists and the next action through those links.
- When naming another document, RFC, PR, or decision record, provide a concrete
  link at the point of discussion, using the canonical source and relevant
  section where useful. Interlink dependencies, parallel proposals, amendments,
  and outcomes instead of duplicating their content. Label planned items without
  real URLs as unsubmitted; never guess a future PR link. Review links and
  anchors with the text and update them when targets move or become available.
- Keep the [RFC book generator](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/generate-book.py)
  working. It discovers RFCs under `text/`; explicit GitHub links in the
  [repository README](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/README.md)
  provide initial access to routine records. Adding them to the book is optional
  follow-on work.
- Coordinate with [purview PR #2](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/2)
  before proposing any change to its sheet-based
  workflow. This RFC does not replace those tabs, change its rating criteria,
  or require historical records to be migrated.

## Initial Rollout And Completion

After the applicable acceptance, confirm a willing meeting-record maintainer,
the permitted public-record scope, and where official records must remain.
Use a routine implementation PR to introduce one newly produced public
agenda/minute and one small linked topic/follow-up record. Readers should be
able to find the evidence or authoritative outcome and the next action without
opening another RFC for routine maintenance.

Acceptance agrees the broader working-artifact scope. It does not rewrite the
repository's [RFC process](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/README.md),
alter formal decision authority, or adopt the separate
charter amendments (planned)
or [future mission (Draft PR #4)](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/4). The following runway is
advisory context only.

## Parallel Review Of Working Method And Future Mission

How the TAC works and what its future responsibilities should be are separate
decisions. This working-method proposal and
[Future TAC Mission, Scope, and Responsibilities (Draft PR #4)](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/4) may be reviewed in parallel under the
[published RFC process](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/README.md#what-the-process-is).
Neither needs the other to be accepted first: this working method can support
the present duties, while the mission can be considered using the current RFC
and official-record arrangements. Acceptance of one does not accept the other.

The subsequent operating-model proposal (planned)
should reconcile the actual outcomes of both
reviews, using the approved working arrangements and distinguishing proposed
responsibilities from those already authorised. Deferring either proposal does
not itself block review or disposition of the other.

## Recommended Initial PR Runway

The table starts with two already-open proposals, linked to their public PRs,
then suggests ten further changes toward the future TAC model. The existing
PRs are related work, not accepted decisions or prerequisites that this RFC
silently adopts. PRs #1 and #2 and the two Draft PRs linked below have actual
GitHub numbers; #5–#12 are illustrative queue positions, not assigned numbers
or a required submission or acceptance order. **Neither the recommended
numbering nor the recommended content is binding or authoritative.** Beyond
the two submitted Drafts, recommended topics remain unsubmitted; their public
links will be recorded when actual proposals exist.

| PR | Topic | Status and intended contribution |
| --- | --- | --- |
| [#1](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/1) | Reference vehicle architecture | Existing open PR: capability-first architecture, project mapping, and a small end-to-end scenario. Coordinate later principles and integration work with this proposal. |
| [#2](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/2) | Project purview rating criteria and process | Existing open PR: evidence-based criteria and a sheet-based review flow. Coordinate later purview changes with this proposal. |
| [#3](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/3) | TAC New Way of Working — this RFC | Submitted Draft, not adopted: agree Markdown/GitHub as the shared working medium, with ordinary records and substantial RFC proposals using their respective review routes. Review in parallel with the mission proposal; neither requires the other's acceptance. |
| [#4](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/4) | Future TAC mission and scope | Submitted Draft, not adopted: propose future responsibilities and authority boundaries, explaining the change from present duties. Review in parallel with this working-method proposal, without adopting it by implication. |
| #5 | Future TAC operating model | Recommended, not submitted: explain how those responsibilities produce owned outputs, review, referrals, and tracked next steps. |
| #6 | Charter amendments | Recommended, not submitted: translate the reviewed future direction into proposed formal wording and the applicable approval route. |
| #7 | Technical ambition level | Recommended, not submitted: describe the intended SDV ambition through code-first evidence, demonstrability, and engineering practice. |
| #8 | Lightweight architecture principles | Recommended, not submitted: develop non-mandatory principles, coordinated with [reference-architecture PR #1](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/1). |
| #9 | Decision records and transparency | Recommended, not submitted: preserve ecosystem reasoning and make material deviations visible to the Steering Committee. |
| #10 | Purview method alignment | Recommended amendment, not submitted as a separate PR: coordinate with existing [purview PR #2](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/2) on evidence safeguards, metadata, and the Markdown review workflow. |
| #11 | Engineering evidence and specialist referrals | Recommended, not submitted: explain useful evidence and the route to the responsible bodies. |
| #12 | Roadmap signals and cross-project moderation | Recommended, not submitted: review project-owned plans and surface dependencies, gaps, and integration opportunities. |

This is a recommended starting runway for discussion. Topics may be reordered,
reworded, split, combined, added, or dropped as the TAC learns and reviews
existing work. Some work may proceed through an amendment to an existing PR,
so actual GitHub numbers and the eventual number of PRs will differ. Every
substantive proposal retains its own consultation, review, and applicable
decision/approval route. Accepting this RFC does not approve the other rows.

The working-method and mission Drafts, followed by the recommended operating
model, establish the future direction and how to work toward it; later items
develop its detailed content.
A small pilot, adoption review, and ongoing reporting are further candidates
and may be brought forward when useful; they are not commitments made by this RFC.

# Drawbacks
[drawbacks]: #drawbacks

GitHub introduces learning and maintenance effort. Adding routine records may
make an RFC-focused repository harder to navigate. Official records can be
duplicated accidentally. Use a small initial scope, clear links to authoritative
sources, and an identified maintainer. No historical migration is required.

# Rationale and alternatives
[rationale-and-alternatives]: #rationale-and-alternatives

Keeping routine records alongside proposals gives readers one starting point.
If maintainers prefer this repository to remain RFC-only, a linked companion
repository is a viable alternative with an extra navigation/maintenance cost.
Keeping the current mix of tools avoids migration effort but leaves the
connections to proposals and next actions less explicit. Giving every note
an RFC number would add ceremony without proposing a substantial change.

# Prior art
[prior-art]: #prior-art

The [destination RFC process](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/README.md)
and [contribution rules](https://github.com/PLeVasseur/sdvwg-tac-rfcs/blob/main/CONTRIBUTING.md)
already establish the proposal workflow, review, and disposition. This RFC
uses those rules for the proposed Markdown working model. The open
[reference-architecture PR #1](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/1)
illustrates substantive technical coordination work; its
[review discussion](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/1#pullrequestreview-5349473965)
raises the need to integrate with official project information rather than
duplicate it. The open
[purview RFC #2](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/2) provides the
concrete sheet-based process with which any later migration must coordinate.
The [Working Group Charter](https://www.eclipse.org/collaborations/working-groups/sdv/charter/)
continues to govern formal committee action.

# Unresolved questions
[unresolved-questions]: #unresolved-questions

- Before disposition: do TAC participants and repository maintainers support
  routine records here or in a linked companion repository? What public-record
  scope is appropriate, and which existing official records must stay elsewhere?
- Before rollout: confirm a willing maintainer and the initial paths/navigation.
- Separate follow-on work: decide whether to migrate any purview records in
  coordination with [PR #2](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/2),
  and whether to add routine records to the book.

# Future possibilities
[future-possibilities]: #future-possibilities

Add link/format checks, optional document exports, and source-based reporting
after the basic workflow is useful. The separately reviewed
[future mission (Draft PR #4)](https://github.com/PLeVasseur/sdvwg-tac-rfcs/pull/4)
and operating model (planned)
can then use these records without depending on a new platform.
