---
title: 'Session 3: Naming Reuse Needs'
authors: [taylor, monica]
date: 2026-03-19
downloads:
  - file: session-3-slides.pdf
    title: Session 3 Slides
---

| Date and time    | March 19, 2026                                                       |
| :--------------- | :------------------------------------------------------------------- |
| **Format**       | Virtual (Zoom)                                                       |
| **Hosts**        | Creative Commons x Continuous Science Foundation                     |
| **Facilitators** | Taylor Campbell [Monica Granados](mailto:monica@creativecommons.org) |
| **Theme**        | Licensing as Infrastructure for Open Science                         |
| **Slides**       | [Session 3 Slides](./session-3-slides.pdf)                           |

The Reuse Incentives Working Group's third session focused on naming the reuse needs that a framework for modular science should address. Building on the friction points surfaced in Session 2, participants articulated twelve needs across four categories and then worked in breakouts to ideate solutions and incentives for the different stakeholders involved in modular research.

## Recap: The Modular Paper Repo

Before the activity, participants revisited the modular paper repo model that frames the working group's scope. A "paper repo" is a shareable collection of research objects built from:

- **Hypothesis headlines** — claim-level containers
- **Panels of evidence** — supporting text, figures, and tables, embeddable or published independently
- **Panel dependencies** — code, datasets, design files, or lab notes that underpin a panel
- **PDF paper** — a traditional paper view of the repository, with dependencies linked out

Because authorship, licensing, and attribution can each operate at multiple levels of granularity — component, panel, or repository — reuse needs look different at each level.

## Activity: Naming Reuse Needs

Participants reviewed and expanded a list of reuse needs grouped into four color-coded categories.

:::{figure} images/reuse-needs.png
:label: reuse-needs
:align: center
Reuse needs named during the session, grouped into publishing for reuse, setting attribution expectations, reuser guidance, and thinking outside of the PDF.
:::

**Publishing for reuse (green)** — knowing **if** and **how** a component can be reused as a primary source, knowing **if** and **how** components can be licensed, and knowing **what** must be done to properly license components.

**Setting attribution expectations (blue)** — tracking credit received as an author, and distinguishing attributions received for components vs. PEs vs. PRs, and for primary vs. secondary sources.

**Reuser guidance (pink)** — knowing **what** a license requires, being able to easily **do** what it requires, and tracking whether a reuser has met those requirements.

**Thinking outside of the PDF (yellow)** — preventing harmful gaming of attributions, access to a formal environment or standard protocol for publishing modular objects, and attribution options during informal sharing.

## Breakouts: Solutions and Incentives

Breakout groups each selected one of the four colors and worked through two prompts: What would be an ideal solution to these needs? What would motivate participation across sharing authors, reusing researchers, repository owners, hosting institutions, technical developers, and the general read-only public?

### Publishing for reuse

Participants emphasized that the problem is less about willingness and more about a lack of information. Most researchers would share if the practical path were clearer.

- Educational resources that cover practical ways to share, what sharing looks like, and the steps to take
- Tools that allow each panel or component to be used and reshared independently, with guidance on how to describe desired reuse
- A menu of licensing options presented in terms of **practical use cases** rather than license names
- Tools that execute the licensing steps directly, or clearly guide authors through them

### Setting attribution expectations

Group discussion centred on attribution working at the level of **evidence statements** — units that carry attribution and aggregate up to the paper repository.

- Structured attribution within components that roll up to the container (e.g. the "paper repo"), with distinct sections for evidence, description, and contributions
- Norms for what information is shared and what downstream reusers should do with it
- A CrossRef or DOI-based API that takes a PID as input and returns the set of other objects that refer back to it
- Participants worked through a concrete scenario: a Paper Repo with various components (e.g. "Panels of Evidence") with different co-authors that credit lab techs and software engineers. When someone cites only the figure, when someone cites only the container, and when someone cites both — what is a fair way to acknowledge the work and the authors involved at each level?

### Reuser guidance

The group returned to a clear principle: **lift the burden on the reuser**. For academics, much reuse is already covered under Fair Use — but accidental violations are common.

- Metadata that travels with content when it is reused, so that license terms are visible at the point of reuse, whether the reuser is a person or a machine
- Compliance drives incentive: when authors see their attribution terms respected, they are more likely to open more content for reuse
- An open question emerged: is tracking compliance actually a reuser's need, or is it more a need for publishers and funders trying to audit use downstream?

### Thinking outside of the PDF

The group explored what sits beyond the traditional paper — both in gaming risks and in sharing contexts.

- Preventing gaming may be impossible to solve entirely. A more productive framing is to **make citations more valuable** — for example, by showing them in context.
- Quantitative citation counts are easily gamed; modular outputs dilute the impact of any single citation. Measuring actual reuse of components, or measuring how much a piece of evidence changed the confidence in a hypothesis, are more meaningful signals.
- Infrastructure pointers: [OXA](https://oxa.dev) for modular publishing; content with actual APIs so both humans and machines can build on top of them; a set of functions AI tools can use; explorations of the counter-factual impact of removing evidence.
- Informal sharing needs attribution too: places to list datasets or "top ten contributions," direct links to Tenure and Promotion criteria or NIH policy, and specialized CVs that surface different kinds of work. There is both appetite and possibility to move informal attribution from possible to normative.

## Cross-Cutting Themes

**Licensing must be presented through use cases, not license names.** Across groups, participants emphasized that the menu of options researchers see should be framed by practical intent.

**Attribution needs to travel with the object.** Whether the reuser is a person, a platform, or an AI tool, license and attribution metadata should remain attached to the modular object across its journey.

**Measurement should shift from citations to reuse.** As research becomes more modular, traditional citation counts capture less of the actual reuse happening downstream. Qualitative and contextual signals matter.

**Informal sharing is the largest untapped surface.** Much real-world reuse happens outside formal publishing, and the systems for attributing that work are not yet normative.

## Next Steps

The working group will carry these named needs into Session 4, turning them into a draft set of recommendations with concrete tactics. Upcoming meetings are scheduled for April 2 and April 16, 2026.

Takeaway reading for participants: [Library and Archives 101: AI and The False Promise of Control](https://authorsalliance.substack.com/p/library-and-archives-101-ai-and-the).
