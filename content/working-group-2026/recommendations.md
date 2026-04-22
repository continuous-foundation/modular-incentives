---
title: Recommendations
authors: [taylor, monica]
date: 2026-04-22
numbering:
  headings: true
---

:::{warning} Preliminary Draft
These recommendations are a **preliminary draft** produced by the Reuse Incentives Working Group between February and April 2026. They are intended to describe ideals and gaps — goal posts for the community — rather than a finished specification. We expect them to evolve as implementations, examples, and feedback come in from the broader research ecosystem. Contributions and refinements are welcome via [GitHub](https://github.com/continuous-foundation/modular-incentives) or the [working group mailing list](https://groups.google.com/a/continuousfoundation.org/g/modular-incentives).
:::

The seven recommendations below emerged from five working group sessions and were pressure-tested against each level of a modular research object — paper repo, hypothesis headline, panel of evidence, individual text/figure/table objects, and panel dependencies. Together they describe what it would take for licensing and attribution to function as infrastructure for reuse in modular science, for both humans and machines. See the [summary](./summary.md) for the arc of the working group and the [next steps](./next-steps.md) for how this work moves forward.

## Reusing

Ensure readers know if and how they can reuse a modular research object as a primary source. It is important that readers feel confident about reusing modular research, so we recommend educational resources that teach practical steps and technical infrastructure that provides visual cues about the reusability of modular objects.

## Sharing and Licensing

Ensure authors know if and how they can share and license modular research objects, and what proper licensing entails. Many are unaware what licensing options exist for communicating how an author wants their modular research to be reused, or how to go about it. It is important to provide comprehensive training, guidance, and automated assistance for licensing research. We recommend the development of a feature, tool, or API that detects, validates, and displays the menu of recognized and available open-source licenses, based on practical use cases, so that publishers can confirm that the license that has been selected is well-registered, including for mixed licenses (e.g. for assemblages with different licenses for sub-components). It should also autocheck and validate bespoke licenses that are submitted separately and suggest a comparable validated license instead.

## Provenance Tracking

Ensure authors and funders have a way to track attribution and reuse of their research. This improves the process of knowing how or where their research is being used. We recommend always providing structured and standardized attribution (i.e., including Title, Author/Funder + with ORCiD or ROR IDs, Source Link, and License Link) in metadata. These values should be available within modular evidence statements and get aggregated up to the whole paper repository. This can also involve using CrossRef or a DOI-based API that receives the PID as input and returns "these other things refer back to that PID", e.g. “government data, public domain;” “author-originated data, with data subject agreement;” “reused from \[DOI]”.

## Attributions, By Object

Ensure platforms have a way to show attributions in context for various modular object types, and for primary vs. secondary sources. When research is presented via modular objects, authorship has the potential to change across levels, so we recommend surfacing context for attribution at all levels and mapping credit to authors and co-authors at each level. This includes exploring direct links to single figure panels to increase the usefulness of their attribution and the payoff for referencing or labeling a specific figure panel, and propagating the 'percentage of contribution' for downstream reuse elements. Norms for mixed-authorship attributions will also be necessary to ensure credit doesn't default only to top-level authors, and distinctions between primary and secondary sources should allow credit to flow to originating authors. Qualitative narratives about the value of components can add meaningful context, helping distinguish between, for example, field data that is effort-intensive to collect and methods code that is easily reused as part of a software library and accumulates many attributions. Attribution counts alone can be easily gamed as performance metrics, limiting the number of attributions per paper is hard to enforce in practice, and fragmentation across platforms can make reuse difficult to track comprehensively.

## License Compliance

Ensure readers have a way to know and easily do what is required of licenses as components are reused. Licenses are easy to violate accidentally, and respected attribution terms increase the likelihood of authors sharing their content for reuse. We recommend defining the mechanisms for metadata that travels with content when it’s reused so that license terms are visible, clear, and actionable at the point of reuse and enables better tracking of publications, especially for AI tools trying to (re)use these knowledge objects. We also recommend a feature or tool that executes the licensing steps for reusers or clearly guides the reuser through the steps, especially for places where data and publications are aggregated (e.g. -xiv sites). This could entail building attribution and other license requirements into RAG systems, and making APIs that make those fields mandatory. This could also be supplemented with surfaced context about what intended uses are covered under Fair Use, where relevant. It is recommended to drive adoption of this by pitching it in alignment with existing use cases of publishers, preprint platforms, and funders.

## Modular Environment

Ensure authors and readers have access to a seamless formal research environment, platform, or standard protocol for easily publishing and reading modular research, with outputs interoperable across platforms. This is what will make modular sharing practical at scale. We recommend it be adopted or built toward modular publishing standards and exchange architectures that tools can interoperate with, like OXA (https://oxa.dev), use API specifications for machines, and be integrated into existing preprint servers and publishing platforms (including RO-Crates or paper-repos). This can also be supplemented with functions or tools that enable human or machine interaction with modular objects to compose and/or annotate them.

## Informal Sharing

Ensure authors and funders have attribution options during informal sharing as well. Informal and social media sharing is where most real-world reuse actually happens, and formal publishing systems no longer fully represent the scope of a researcher's work. We recommend leveraging the existing appetite and possibilities to move informal attribution from possible to normative, with exploration of ways to bootstrap informal sharing into the existing publishing ecosystem and leveraging. For example, explore how some of these concepts can work without a traditional journal having to change anything and while maintaining author contribution profiles (like Stack Exchange or Github profiles) to make new contribution types more visible, how specialized CVs can have different ways to highlight existing research to qualify for tenure or promotions, or how informal contributions can be captured and presented, including for example, top ten contributions.
