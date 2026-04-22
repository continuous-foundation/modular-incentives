---
title: Next Steps
authors: [taylor, monica, rowan, courtney]
date: 2026-04-22
---

The [recommendations](./recommendations.md) produced by the working group are a starting point. To move them from aspiration to adopted practice, they need to be socialized, translated into standards, and integrated with the tools researchers and publishers already use.

## Share the work and build standards

The first job is getting these recommendations in front of the people who can act on them — publishers, preprint servers, funders, infrastructure builders, and the teams building the next generation of editing and publishing tools. Creative Commons and the Continuous Science Foundation will drive this through their respective communications channels, library networks, and the [working group mailing list](https://groups.google.com/a/continuousfoundation.org/g/modular-incentives).

## OXA as a point of coordination

A recurring theme across the sessions was the need for a coordination point — a place where these recommendations can be translated into interoperable technical specifications rather than re-implemented in parallel across platforms. [OXA](https://oxa.dev) is well positioned to serve that role. It is community-driven, RFC-based, and already being evaluated by tooling teams in both educational and scientific publishing workflows that are directly asking for this kind of object-level licensing and attribution work.

Several publishing organizations are already moving in this direction. [eLife](https://elifepathways.org/partnerships/) is partnering around OXA to support modular publishing pathways, and [openRxiv](https://openrxiv.org) — the nonprofit stewarding [bioRxiv](https://www.biorxiv.org) and [medRxiv](https://www.medrxiv.org) — is helping steer OXA and plans to translate its ~500,000 preprints into the format, partnering with [Curvenote](https://curvenote.com) on the translation work. Object-level licensing and attribution landing in OXA would therefore reach a substantial existing corpus rather than starting from zero.

**Technical next step: an OXA RFC on metadata.** CSF and CC will open an RFC on OXA proposing a metadata schema for object-level licensing, attribution, and provenance that operationalizes these recommendations. Working group members will be invited to collaborate on the RFC, contribute use cases, and test it against the editing and publishing tools already requesting it.

## Educational activities

Several recommendations — particularly around authors knowing **if** and **how** to share and license their work — depend on educational resources that do not yet exist at scale. The working group flagged educational activities as a distinct track of work that will require dedicated funding to produce high-quality materials: authoring guides, licensing walk-throughs, real examples of modular reuse, and the schematic explanations that make mixed-licensing concepts tractable for researchers.

## Broadening the use cases

The framing used in this working group — modular objects, paper repos, panels of evidence, reuse signals — is considerably broader than scientific publishing. We heard consistent feedback that the same concepts apply wherever structured content is authored, reused, and attributed at the component level. We think the surface is wide.

Educational publishing is the most immediate adjacent use case: textbooks, open educational resources, course materials, problem sets, lecture slides, and interactive learning objects all face the same component-level reuse and attribution challenges modular science does. A figure from an open textbook, a problem from a shared assessment bank, or a notebook in a course repository should carry the same licensing and attribution signals as a figure in a paper.

Similar dynamics appear in technical documentation, policy briefs and evidence synthesis, journalism and fact-checking, software documentation, and standards work — any setting where modular content moves between contexts and needs to carry its provenance with it. Expanding the framing to explicitly cover these use cases broadens both the audience for this work and the set of tools that can adopt it.

## Guidance by participant

Translating these recommendations into practice takes different actions from different parts of the ecosystem. The framings below are starting points, not prescriptions — we expect them to sharpen as implementations land.

**Funders.** Recognize modular research outputs — datasets, code, figures, notebooks — as first-class outputs in grant reporting and evaluation. Include object-level licensing and attribution expectations in open-science policies. Fund the educational resources and tooling this work depends on.

**Publishers.** Support component-level licensing and attribution in article and preprint pipelines. Expose license and attribution metadata in APIs. Where mixed licenses apply across sub-components, make them unambiguous to readers. Adopt license-chooser tooling that accounts for object type and the enclosing repository context.

**Researchers.** As authors, license modular outputs explicitly and describe how you want them reused. As reusers, attribute at the component level, including in informal sharing. Use persistent identifiers for the objects you produce and depend on.

**Preprint servers.** Treat modular objects as first-class, not just attachments to a PDF. Expose object-level license and attribution metadata in APIs. Consider sensible default licenses for aggregation contexts, and build in validation to catch unregistered or bespoke licenses early.

**Infrastructure.** Support hierarchical persistent identifiers that link objects to their panels, paper repos, funders, and contributors. Expose reverse-citation APIs — given a PID, return the things that refer back to it. Align metadata schemas with emerging object-level attribution work rather than paper-shaped ones.

**Tool-builders.** Ensure licensing and attribution metadata travels with content by default. Make compliant reuse easier than copy-and-paste. Surface licensing signals visually at the point of reuse. Integrate with OXA, RO-Crate, and related packaging efforts so objects carry their reuse signals across tools.

## Adoption in existing projects

Rather than ask the ecosystem to add one more standard, the working group emphasized hooking into what already exists. Early candidates for adoption include tools already aligned with modular publishing:

- [**Quarto**](https://quarto.org) — a scientific and technical publishing system that treats figures, tables, code, and notebooks as composable modular objects
- [**MyST**](https://mystmd.org) — a structured markdown ecosystem from [Project Jupyter](https://jupyter.org) for scientific writing with first-class support for cross-references, executable content, and modular publishing workflows
- [**Discourse Graphs**](https://discoursegraphs.com) — a framework for modular scientific argumentation that makes claims, evidence, and questions independently citable and reusable
- [**Stencila**](https://stencila.io) — authoring and publishing infrastructure for executable, machine-readable research documents
- [**Curvenote**](https://curvenote.com) — a collaborative authoring and publishing platform for modular, executable, and citable scientific content
- [**Octopus**](https://www.octopus.ac) — a publishing platform that splits the scientific record into modular, independently citable units (problems, hypotheses, methods, results, analyses, interpretations, and real-world applications)

[**MIRA**](https://www.mira.science/) is planning an implementation-focused workshop as an upcoming coordination space for invited researchers to move these recommendations into practice.

Beyond modular-native tools, adoption in the most widely used authoring environments — **Google Docs, Microsoft Word, and LaTeX** — matters for reach. The extensibility surface in these tools is narrower, but not absent.[^word-extensibility] Finding workable entry points for object-level licensing and attribution in mainstream authoring environments is an open area of work.

[^word-extensibility]: Reference management software — Zotero, Mendeley, EndNote, Paperpile, and others — has long demonstrated that substantial metadata-aware features can be added to Word, Google Docs, and LaTeX through add-ins, plugins, and macro systems. The same extensibility pathways should support object-level licensing and attribution features, even if the integration is less seamless than in modular-native tools.

## How to get involved

The work continues beyond these five sessions. If you would like to contribute to the OXA metadata RFC, the educational materials, or adoption in a specific tool or platform, please reach out via the [working group mailing list](https://groups.google.com/a/continuousfoundation.org/g/modular-incentives) or [open an issue on GitHub](https://github.com/continuous-foundation/modular-incentives).
