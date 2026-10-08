# Product design playbook

How I take a product from a vague request to something live, and keep it getting better. Eight steps, each with what I actually do, a real example from my work, and a template you can copy.

By [Miguel Clavel](https://github.com/miguelclavel), Senior Product Designer at U.S. News & World Report, working on insurance quotes, credit cards and loans, where getting it wrong costs someone real money or real time.

| Step | In one line | Template |
| --- | --- | --- |
| [1. Frame the problem](#1-frame-the-problem) | Make sure the team is answering the right question | [Problem brief](templates/problem-brief.md) |
| [2. Find the evidence](#2-find-the-evidence) | Let what people do pick the direction | |
| [3. Explore fast, with AI, and check it](#3-explore-fast-with-ai-and-check-it) | Speed from AI, judgment from you | [AI review checklist](templates/ai-review-checklist.md) |
| [4. One decision at a time](#4-one-decision-at-a-time) | Ask for less at once | |
| [5. Build the system, not just the screen](#5-build-the-system-not-just-the-screen) | Make it work without you in the room | |
| [6. Test on a cadence](#6-test-on-a-cadence) | Turn isolated tests into shared learning | [Experiment plan](templates/experiment-plan.md) |
| [7. Check before it ships](#7-check-before-it-ships) | Every state, every screen size, every keyboard | [Design QA](templates/design-qa-checklist.md) · [Launch checklist](templates/launch-checklist.md) |
| [8. Launch, then keep listening](#8-launch-then-keep-listening) | The work after launch is the product | [The short version](templates/case-study-short-version.md) |

---

## 1. Frame the problem

Everyone sees the final interface. Fewer people see the question that made it worth building.

A weak question: *"How might we redesign this dashboard?"*
A stronger one: *"Why are users opening the dashboard and still calling support?"*

Before I open Figma, I ask:

1. What behavior are we trying to change?
2. What evidence tells us this is the real problem?
3. What happens if we do nothing?

Problem framing means separating symptoms from causes, working out whose problem matters most, defining what success should change, and knowing what not to design. AI makes this more important, not less: it can generate ten flows before lunch, and solve the wrong problem at incredible speed when the brief is wrong.

**Template:** [Problem brief](templates/problem-brief.md)

## 2. Find the evidence

Most of my work starts with what people actually do, not what we assume they do.

**Example.** An insurance hub was a 9,500 pixel list of links with no way to start a quote. Heatmaps showed 26.6% of mobile clicks were landing on things that weren't links: people were trying to act and the page gave them nowhere to go. The rebuild put a quote form first, and the site audit score went from 66 to 88 while about 120 production links stayed intact. [The case study](https://miguelclavel.com/work/insurance-landing-page?utm_source=github&utm_medium=playbook)

What I use: competitive analysis, user interviews, journey mapping, heatmaps and scrollmaps, analytics, and usability testing. The point of all of them is the same: replace an opinion with something you can show the room.

## 3. Explore fast, with AI, and check it

I use AI daily and hands on: research synthesis, exploring directions, and building working prototypes rather than pictures of them. It cut my synthesis time by about 40%. Claude, Claude Code, Claude Design, ChatGPT, Gemini, Figma Make and v0 are all part of the kit. It hasn't replaced the judgment part.

AI failures are rarely loud. The dangerous ones are quiet, so I look twice at:

- **Numbers in summaries.** Every statistic gets traced back to its source before it reaches a stakeholder.
- **The emotional register.** Drafts about money, health or layoffs often arrive one level too cheerful.
- **Made up specifics.** Fake feature names, plausible but wrong dates, references to things that don't exist.
- **What it left out.** AI answers the prompt. It doesn't volunteer the risk you forgot to ask about.

Trust the speed. Audit the substance. Both, always.

**Template:** [AI review checklist](templates/ai-review-checklist.md)

## 4. One decision at a time

A thread through most of my work: helping people understand information, compare options, weigh tradeoffs, and act with confidence. In money products that usually means asking for less at once.

**Example.** A car insurance quote asked people 30 questions before giving them anything. It became a conversation with one clear question at a time: 23 form fields turned into 19 questions across 5 named stages, answered by tapping instead of typing, with every answer editable. No language model at runtime; it's the design ground agentic products stand on: intent, progressive disclosure, readable states, recovery, and a clear next step. [The case study](https://miguelclavel.com/work/auto-insurance-conversational-flow?utm_source=github&utm_medium=playbook)

## 5. Build the system, not just the screen

A design only scales if people can use it without asking you.

**Examples.** A brand nobody owned: I wrote the 54 page guide, took it through senior stakeholders and legal, then turned it into rules teams could follow. At BLU Products, more than 20 phone launches ran off one shared set of components, so a late spec change didn't mean starting over. At U.S. News I own the design system, interaction standards and the WCAG accessibility guardrails across the financial verticals.

## 6. Test on a cadence

One A/B test answers one question. A cadence builds a team's judgment.

**Example.** A monthly A/B testing review turned isolated experiments into shared learning: experiment operations, synthesis, decision communication, and a reusable testing cadence. Tests run against the numbers the business cares about, like click through rate, quote completion and lead generation. [The case study](https://miguelclavel.com/work/monthly-testing-review?utm_source=github&utm_medium=playbook)

**Template:** [Experiment plan](templates/experiment-plan.md)

## 7. Check before it ships

Every state (empty, loading, error, success), every screen size down to a phone, and every path a keyboard can take. Then the boring parts that decide whether anyone sees the work: security, search, speed.

**Example.** After launching my chat portfolio I ran it against one checklist covering security, search, accessibility, UX and speed, and fixed what failed: page titles and descriptions cut to length, contrast, reflow at 320 pixels, keyboard menus, private pages kept out of search.

**Templates:** [Design QA checklist](templates/design-qa-checklist.md) · [Launch checklist](templates/launch-checklist.md)

## 8. Launch, then keep listening

Launch day is when the real feedback starts.

**Examples.** Three things broke when I relaunched miguelclavel.com, and none of them were design: the host ran out of build credits mid launch week, the first deploy on the new host uploaded the git history, and a caching rule froze my own code in visitors' browsers. My chat portfolio logs the questions it can't answer yet; every week I write those answers and add each question to a test bank of more than 2,000. The first two notes from a real visitor were fixed the same day. [The build log](https://github.com/miguelclavel/chat-portfolio/blob/main/BUILD-LOG.md)

And when it's done, write it up so someone reading for 30 seconds still gets it.

**Template:** [The short version](templates/case-study-short-version.md)

---

The templates are free to copy and adapt, under the MIT license. Case study material belongs to the companies named and is shown for portfolio purposes. More of my work: [miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=playbook) · [GitHub](https://github.com/miguelclavel).
