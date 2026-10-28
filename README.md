# Reverse Engineer Strategy

**RES**

**Reverse engineer your competitors’ strategy from what they ship.**

Give RES a competitor. It investigates their releases, documentation, pricing and public communications to uncover who they're targeting, the bets they're making and where their strategy is vulnerable.

Use it to understand a competitor's direction, investigate a suspected shift or turn scattered announcements into a clear strategic assessment.

Every conclusion comes with evidence, a challenge and a confidence level.

[Get started](#get-started) · [The four tests](#the-four-tests) · [Example verdict](#example-verdict) · [Read the skill](SKILL.md)

---

## The four tests

A strategy should make four choices clear. RES tests each against what the company actually does.

| Test | The question | The warning sign |
| --- | --- | --- |
| **Customer** | Who are they choosing to win with? | An audience too broad to guide decisions. |
| **Bet** | What will make those customers choose them? | A feature list with no explanation of why it wins. |
| **Edge** | Why are they particularly well placed to deliver? | An advantage equally available to competitors. |
| **Trade-off** | What are they choosing to do less of, or decline? | Every opportunity becomes a priority. |

The useful part is the gap between the story and the decisions. A company can explain its strategy beautifully while its releases, pricing and priorities tell a different story.

## Get started

Install with the [skills CLI](https://skills.sh/docs/cli):

```bash
npx skills add justshipai/res
```

Choose your agent when prompted. Then ask:

```text
Use RES to reverse engineer Linear's strategy over the past six months.
```

Or give a more specific question:

```text
Use RES to assess whether Notion's recent releases reinforce a coherent
strategy. Where are its customer choices and trade-offs least convincing?
```

For an agent without a skill installer, give it [SKILL.md](SKILL.md) and ask it to follow the instructions. It needs web search or browsing access to research current evidence.

RES is an instruction-based skill. No API keys, server or custom runtime required. Your agent's normal usage costs still apply.

## What you get

- **A strategic thesis:** the choices that best explain the company's actions.
- **Four evidence-backed tests:** inferred choices, dated sources, alternative explanations and confidence.
- **A candid verdict:** whether the choices reinforce one another, the weakest link and its consequence.
- **A signal to watch:** what would strengthen or overturn the assessment.

Run it again later to see which conclusions strengthened, weakened or changed.

## Example verdict

*Illustrative, using a fictional company:*

> Northstar has a clear customer and a coherent bet: help design agencies move from reusable project setup through client feedback, approval and handoff.
>
> Its weakest link is **Edge**. These features could make the product useful without giving customers a compelling reason to choose it over competitors. The roadmap supports the proposition; the evidence for an advantage is weaker.
>
> The broad “AI for every industry” blog post is loose positioning. It doesn't establish erratic execution when six months of releases consistently serve agencies.
>
> **Watch next:** evidence that agencies repeatedly choose and renew Northstar specifically for its integrated delivery workflow.

## Where it looks

Release notes, help and developer documentation, pricing and packaging, company and founder posts, customer stories, partnerships and job adverts.

RES follows sequences rather than counting launches. It checks primary sources, avoids counting the same announcement several times, and distinguishes a launch from a later documentation update.

## Why trust the verdict?

RES is designed to challenge its own interpretation. It tests whether a supposed strategic move could be maintenance, competitive catch-up, a small experiment or an isolated customer request.

It can call a strategy poorly defined, fragmented or erratic. It also has to show why. Broad positioning alone isn't proof of confused execution, and gaps in public information aren't proof that no strategy exists.

Expect a reasoned assessment, not access to internal intent. Shipping doesn't prove adoption. A plausible bet doesn't prove commercial success. Missing sources and uncertainty stay visible.

## Contribute

Found a weak inference or a useful source the skill missed? Open an issue with the prompt, relevant evidence and what the assessment got wrong. Improvements should sharpen the judgement while keeping the skill compact.

## Inspiration

The name is inspired by [REA](https://github.com/morluto/rea). REA investigates how software works; RES investigates the strategic choices behind what a company builds. RES is an independent project.

Built by [JustShipAI](https://github.com/justshipai).
