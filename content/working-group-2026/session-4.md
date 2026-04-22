---
title: 'Session 4: Refining Our Guidance'
authors: [taylor, monica]
date: 2026-04-02
downloads:
  - file: session-4-slides.pdf
    title: Session 4 Slides
---

| Date and time    | April 2, 2026                                                        |
| :--------------- | :------------------------------------------------------------------- |
| **Format**       | Virtual (Zoom)                                                       |
| **Hosts**        | Creative Commons x Continuous Science Foundation                     |
| **Facilitators** | Taylor Campbell [Monica Granados](mailto:monica@creativecommons.org) |
| **Theme**        | Licensing as Infrastructure for Open Science                         |
| **Slides**       | [Session 4 Slides](./session-4-slides.pdf)                           |

The Reuse Incentives Working Group's fourth session turned the reuse needs named in Session 3 into a draft set of recommendations with concrete tactics, working toward the group's third goal: producing a document with a framework and recommendations for modular science reuse.

Participants reviewed a consolidated set of recommendations, discussed what was missing and what felt most urgent, and shaped the framing of the document as a whole — its audience, its relationship to existing initiatives, and how it should be organized for different readers.

## Key Terms

The session opened by anchoring shared vocabulary for the document:

- **Sharing** — publishing your work so that others can access, use, share, and/or build upon it
- **Reuse** — accessing and using, sharing, and/or building upon someone else's work
- **License** — a set of terms that specify how others can use, share, or build upon your work
- **Attribution / Citation** — credit given to the original creator of a work when it is being reused

## Activity: Our Recommendations

Participants reviewed a consolidated set of recommendations distilled from the twelve reuse needs named in Session 3. Two prompts guided discussion: **what is missing?** and **which of these needs feels most urgent or familiar to you in your work?**

The recommendations, with their tactics, are summarized below.

### Ensure readers know if and how they can reuse a component as a primary source

So that researchers reuse confidently rather than avoiding reuse or getting it wrong.

- Educational resources for authors and readers on practical ways to share work and the steps to take
- Open access / CC BY licensed tools that allow each research component (e.g., figure or text panel) to be used and reshared, with APIs linked to DOIs or other indexes
- Education on how to describe how a component should be reused
- In-line citations or marks on the paper notifying readers that a component can be reused
- Provenance labels, e.g. "government data, public domain"; "author-originated data, with data subject agreement"; "reused from [DOI]"

### Ensure authors know if and how they can share and license modular components

Because many authors and publishers are unaware of what options exist or how to apply them.

- Training and guidance on licensing options
- A feature or API that detects, validates, and displays the menu of recognized open-source licenses, based on practical use cases — including mixed licenses for assemblages with different sub-component licenses
- APIs that auto-check and validate bespoke licenses and suggest a comparable validated license instead
- Tools that execute the licensing steps or provide clear guidelines
- Default licenses applied automatically, especially in aggregation sites (e.g. -xiv servers)

### Ensure authors and funders can track attribution and credit received

Because otherwise it is hard to know where work is being used.

- Structured, standardized attribution (Title, Author/Funder with ORCiD or ROR IDs, Source Link, License Link) within evidence statements that aggregate up to the paper repository
- Attribution norms for the information that is shared
- CrossRef or DOI-based APIs that accept a PID and return references back to that PID

### Ensure authors and funders can distinguish attributions across levels

Because authorship often happens across components, panels of evidence, and paper repositories, and primary vs. secondary source distinctions matter.

- Supported citation at multiple levels, with the ability to map credit to authors and co-authors at each level
- Norms for mixed-authorship attributions that avoid defaulting only to top-level authors
- Distinctions between primary and secondary sources so credit flows to originating authors

### Ensure readers can easily know and meet what a license requires

Because licenses are easy to violate accidentally, and respected attribution terms increase the likelihood of authors sharing content for reuse.

- Metadata that travels with content when it is reused, so license terms are visible, clear, and actionable at the point of reuse — especially for AI tools
- Building these fields into RAG systems and making APIs with those fields mandatory
- Working with publishers and preprint servers to build metadata schemas that enable better tracking and automated reporting
- For academics, surfacing context about which uses are covered under Fair Use

### Ensure readers can track whether they met the license requirements

- Drive adoption by aligning with existing use cases of publishers and funders

### Ensure platforms can show citations in context

Because citation counts alone can be gamed, and as research becomes more modular the impact of a single citation will diminish.

- Linking directly to a single figure or panel to increase the value of a citation at that level
- Measuring actual reuse of components in addition to citation quantities
- Qualitative stories that distinguish, for example, effort-intensive field data from methods code that accumulates many citations as part of a software library
- Propagating a "percentage of contribution" for downstream reuse elements

Open considerations raised: limited reward for data reuse undermines incentives to share, platform fragmentation makes reuse hard to track comprehensively, and limiting citations per paper is hard to enforce while leaving other forms of gaming in play.

### Ensure access to a seamless modular research environment

Because a formal platform or protocol is what will make modular sharing practical at scale.

- Adopt or build toward modular publishing standards and exchange architectures like [OXA](https://oxa.dev)
- Develop an API specification for machines
- Integrate modular publishing into existing publishing platforms and preprint servers
- Tools that provide places to compose and annotate modular objects
- Explore the counter-factual impact of removed evidence — with care around the potential political weaponizing of replication and open-data practices
- Engage evidence-based policy practitioners in fields like public health, climate change, and environmental pollution
- Develop functions that AI can use to interact with and build on modular research outputs
- [RO-Crates](https://www.researchobject.org/ro-crate/) or paper repos with real APIs and tools to build on top of

### Ensure attribution options during informal sharing

Because informal and social-media sharing is where much real-world reuse happens, and formal publishing no longer fully represents a researcher's work.

- Places and ways to list datasets or other informal contributions, such as "top ten contributions"
- Direct links to Tenure and Promotion criteria or NIH policy
- Specialized CVs that surface different kinds of work
- Move informal attribution from possible to normative by leveraging existing appetite
- Bootstrap into the existing publishing ecosystem — concepts that work without traditional journals changing anything
- Author impact and contribution profiles, similar to Stack Exchange or GitHub

## Closing Discussion

Several questions shaped how the document will be sharpened in subsequent drafts.

**A stepwise framing for reuse.** Participants asked what distinguishes recommendation 1 (readers knowing if they can reuse) from recommendation 5 (readers knowing what the license requires), and how both relate to recommendation 2 (authors licensing their work). The group agreed these are two sides of the same coin — whether the reuser needs to attend to a license depends on what came before it — and that a stepwise presentation would reduce confusion:

1. **Make it modular** — possibility, supported by education
2. **Make it licensed** — the responsibility of the creator
3. **Know that you can reuse it** — the need of the reader

**The machine perspective is missing.** Participants noted the document does not yet speak to the machine or API layer. While this framework itself may not contain technical specifications, it should link to projects attempting that work — JSON schemas, programmatic APIs, and machine-readable licensing and attribution. Examples and references to implementations can be added as the draft develops.

**Alignment with existing systems.** Participants emphasized building bridges to existing initiatives rather than proposing parallel efforts — particularly around alt-metrics, metadata schema best practices, and attribution standards. A relevant starting point raised in chat was "[A call for broadening the altmetrics tent to democratize science outreach](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3003010)".

**Goal posts or implementation pathways?** The consensus was to frame the document as a foundational piece describing ideals and gaps, which can then connect to operationalized efforts and inform future technical specifications. Several participants suggested organizing the recommendations by role — writing research, reusing research, crediting, funding — potentially as a table or visual, so different audiences can navigate to what applies to them.

**Priority areas.** Urgent items surfaced included finding and tracking where content ends up after reuse, addressing "AI-washing" of open source repositories, and norm-setting around attribution and provenance from input to output across AI workflows. As one participant framed it: we cannot stop bad behavior, but we can incentivize good behavior.

**Socialization.** The working group will leverage Creative Commons and Continuous Science Foundation communications, library networks, and the [mailing list](https://groups.google.com/a/continuousfoundation.org/g/modular-incentives) for asynchronous discussion.

## Implementations in Motion

Participants are invited to contribute examples of related initiatives. Initial references include:

- [MIRA](https://www.mira.science/) — with an implementation-focused workshop planned for June 2026
- [OXA](https://oxa.dev/) — a technical specification for modular scientific content, developed through a community RFC process
- [RO-Crate](https://www.researchobject.org/ro-crate/) — a research object packaging standard

A first set of priority use cases is emerging to anchor the implementations section: reusing a figure or panel, reusing a dataset or notebook, and citing a component inside a larger work.

## Next Steps

The working group will hold its final session on April 16, 2026, to operationalize the recommendations across the different levels of modular research object, discuss how to socialize the framework, and close out the spring 2026 series.

Takeaway reading for participants: [eLife receives Wellcome boost to build open publishing ecosystem](https://elifesciences.org/).
