---
title: 'Session 5: Brainstorming By Object'
authors: [taylor, monica]
date: 2026-04-16
downloads:
  - file: session-5-slides.pdf
    title: Session 5 Slides
---

| Date and time    | April 16, 2026                                                       |
| :--------------- | :------------------------------------------------------------------- |
| **Format**       | Virtual (Zoom)                                                       |
| **Hosts**        | Creative Commons x Continuous Science Foundation                     |
| **Facilitators** | Taylor Campbell [Monica Granados](mailto:monica@creativecommons.org) |
| **Theme**        | Licensing as Infrastructure for Open Science                         |
| **Slides**       | [Session 5 Slides](./session-5-slides.pdf)                           |

The Reuse Incentives Working Group's fifth and final session focused on operationalizing the framework: taking each of the seven recommendations and thinking through what they look like at each level of a modular research object — paper repo, hypothesis headline, panel of evidence, individual text/figure/table objects, and panel dependencies.

The goal of the session was to pressure-test the recommendations against concrete objects, surface where licensing and attribution operate differently across levels, and identify the technical specs, incentives, and actors that matter at each layer.

## The Seven Recommendations

Participants worked from a final set of seven recommendations that consolidate the tactical work of Session 4:

1. **Reusing** — ensure readers know if and how they can reuse a modular research object as a primary source.
2. **Sharing and licensing** — ensure authors know if and how they can share and license modular research objects, and what proper licensing entails.
3. **Provenance tracking** — ensure authors and funders have a way to track attribution and reuse of their research.
4. **Attributions, by object** — ensure platforms have a way to show attributions in context for various modular object types, and for primary vs. secondary sources.
5. **License compliance** — ensure readers have a way to know and easily do what is required of licenses as components are reused.
6. **Modular environment** — ensure authors and readers have access to a seamless formal research environment, platform, or standard protocol for easily publishing and reading modular research, with outputs interoperable across platforms.
7. **Informal sharing** — ensure authors and funders have attribution options during informal sharing as well.

## Activity: Brainstorming by Object

For each recommendation, breakout groups considered how it lands at each modular level. The patterns below draw out the most concrete threads from that discussion.

### Reusing: licensing signals across levels

A recurring concern was how a license set at a "higher" level of the paper repo relates to the components inside it. If a paper repo is CC BY, does that apply to every panel and figure, or can components carry more restrictive or less restrictive licenses of their own?

Participants suggested a **visible licensing signal that travels with the reader** — a badge, sticker, or panel that stays consistent across levels, making mixed licensing unambiguous. Operationalizing this will require examples, schematics, and visual explanations that show how modular objects can be composed without losing citations, attribution, or licensing.

### Sharing and licensing: a license chooser for modular objects

Creative Commons already provides a license chooser. Participants proposed extending it to account for both the **type of object** being shared and the **context of the repo** it sits in — for example, if a repo carries a CC BY-ND license, the chooser should constrain what licenses can be applied to individual components inside it.

A more speculative idea: a standard for embedding a license identifier directly into a file — a specific tag or signature appended in a known location — so that any tool can detect the applicable license without relying on external metadata. Platform independence was the motivator.

### Provenance tracking: the essential incentive

At the paper-repo level, citation-tracking mechanisms are already robust. The interesting territory is inside the repo — the ability to formally cite specific claims, evidence, or components from within a larger work and track those citations individually.

> The ability to track reuse is the essential incentive for authors to make their content available in modular form. Without this ability, there may be a disincentive — if the modular system makes it too easy and attractive to reuse components without proper attribution.

Participants suggested an automated tool that accepts a DOI or other identifier and returns several attribution formulations: how to cite the object, how to reference it in a methods section, how to mention it in an input-availability statement. Reducing the friction of correct citation raises the rate of correct citation.

### Attributions, by object: schematic guidance

At the paper-repo level, this recommendation rides on existing citation practice for scientific papers. Further down, it gets more interesting.

Participants noted that the **panel of evidence** level is where the recommendation meets implementation and becomes an entry point for training. Schematic diagrams — wireframes, brand-guideline-style references — would help communicate what information to show and how. For individual text, data, and figure objects, unambiguous guidance is needed on **which component should receive attribution**: text usually attributes to its immediate container; data attributes to the surrounding panel dependency; figures may need a combination of the data and code that produced them.

For panel dependencies specifically, participants pointed to the need for **standardized metadata** (README, [CRediT](https://credit.niso.org) authorship info) and PIDs for each element — PIDs that support hierarchical linking up to the panel, paper repo, and funders.

### License compliance: easier than copy-and-paste

The critical observation: at the smallest level of content — a text block, a figure, an equation — **compliant reuse must be easier than copy and paste**. Copy and paste strips metadata; that is the default behavior people already know. Any system that requires more effort than copy-paste to reuse compliantly will lose.

License and attribution information must travel with the content by default, not as an opt-in layer.

Participants also raised an open question at the hypothesis-headline level: is it appropriate to license at this level? Does a hypothesis attract copyright? Who owns it? Attribution may still matter for sharing norms and provenance even where copyright does not apply — a different vehicle from traditional licensing.

### Modular environment: a "PaRHub" for paper repos

Participants imagined a **paper-repo hub** — a platform for hosting, versioning, and citing paper repos the way GitHub hosts code repositories. In an [OXA](https://oxa.dev) framing, this is about packaging content so that a paper repo can live in git, a storage bucket, or a supplemental zip — interoperating with existing journal and preprint infrastructure rather than replacing it.

At other levels:

- **Hypothesis headlines** — structured like a README, with identifiers that link upward to the paper repo and downward to supporting evidence, and with machine-readable semantic relationships so the evolution of a claim over time can be followed. Hypotheses evolve, split, and transform; representing those relationships matters.
- **Panel of evidence** — a modular unit linking a claim to the specific text, figures, tables, or analysis that supports it, via persistent identifiers. Panels may need to be referable from other paper repos, either as dynamic references or as copies — similar to submodules in git.
- **Individual text/data/figure objects** — files in a folder of panels, each with its own persistent identifier.
- **Panel dependencies** — open question: are they dynamic references, copies, or forks?

### Informal sharing: the smallest objects are the entry point

For a paper repo, informal sharing mostly means linking readers back to the full work from wherever they arrive. The interesting entry points are further down.

Individual text, data, and figure objects are the most likely informal entry points — a figure shared on social media, an equation pasted into a thread, a dataset linked from a blog post. Panel dependencies offer a different angle: they could be carried by an individual to "show the work" and demonstrate trust and transparency, particularly for fact-checkers.

## Closing

The working group closed by revisiting its purpose:

> We brought our differing roles and lived experiences to the shared work of reimagining research beyond traditional research outputs and shifting behaviours toward the reuse of modular research outputs.
>
> Clear, open licensing for modular research ensures it can be responsibly reused, attributed, and integrated by both humans and machines.

The recommendations, tactics, and object-level brainstorming from this session will be synthesized into a final framework document — **Recommendations for Licensing and Attribution in the Context of Modular Science Reuse (by both Humans and Machines)** — intended to serve as a foundation for subsequent technical specifications, implementations, and socialization across the research ecosystem.

Asynchronous discussion continues on the [working group mailing list](https://groups.google.com/a/continuousfoundation.org/g/modular-incentives), and participants are invited to contribute examples and implementations as the document is finalized.
