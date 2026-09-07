# I built a Super Mario–style game to teach enterprise customers how to use AI

*And it won my region's Customer Zero Award for applied AI at work — August 2026.*

Try it! Play https://super-agent-run-eng-ver.vercel.app

---

## The problem I kept seeing in AI workshops

Every AI enablement workshop I've run — and I've run a lot of them at Korean enterprises — starts the same way. Everyone in the room agrees AI is useful in the abstract. Nobody disagrees with the demo. And then almost nobody applies it to their actual work when they get back to their desk.

The standard workshop format is the problem. A demo is one-directional. The audience watches, nods, and leaves without ever having *tried* anything themselves. No rehearsal, no failure, no muscle memory. Just "yeah, that looked good."

So I stopped running that kind of workshop.

## Why a game — and why Super Mario specifically

A game solves two things at once.

The first is obvious: it replaces watching with doing. Players make a decision every few seconds, fail, retry, and build a sense of what works. That's the exact loop missing from a one-shot demo.

The second is the part I put more thought into. I could have made a plain quiz or a leaderboard app — those exist, and they mostly get ignored. I chose Super Mario as the aesthetic on purpose. In Korea, Super Mario isn't just a game; it's a shared cultural reference every office worker recognizes instantly — from the twenty-somethings on their first project to the executives in the back row. Zero explanation needed. The moment the coin sound plays, the room is already engaged. That saves the ten minutes I'd otherwise spend selling people on the format.

The metaphor lands, too: manual work is the enemy, AI is the power-up. You *feel* the difference between the two instead of just hearing it argued.

## What actually got built

`super-agent-run` is a mobile web game deployed on Vercel with an Upstash Redis leaderboard. Built with **Claude Code** — which is itself the point: a Solution Engineer with no formal software-engineering background can now ship a working, customer-facing tool without a dev team behind them.

Three roles, three URLs:

- **Player** — runs the game on their phone. Work pain points appear as enemies and bosses. To defeat one, the player chooses between "the manual way" and "the AI way." Every correct AI answer reveals a real Salesforce product screen — Agentforce, Slack, Sales Cloud, Tableau, Data Cloud — mapped to that specific pain point. Coins accumulate.
- **Host** — projects a live leaderboard on the big screen. Names climb in real time. Late arrivals want in.
- **Admin** — swaps question wording and product screenshots per workshop through a back-office, so the same engine works for a sales team, a finance team, or an executive briefing without a code change.

Two variants ship in the repo: a 20-question full deck and a 7-question workshop cut. Both share the same leaderboard, so the shorter version stays fair.

Code (English version): [chanyeonkim-lab/super-agent-run-v2](https://github.com/chanyeonkim-lab/super-agent-run-v2)

## The result

The tool won my region's **Customer Zero Award** — internal recognition given to the Solution Engineer who most effectively applied AI to their own work.

The bigger takeaway isn't the award. It's that a solution engineer can now design, build, and deploy the actual tool a customer experiences — because Claude Code has moved the ceiling. Enablement stops being a slide deck. It becomes something you ship.

This sits alongside a company-wide Claude "vibe coding" training I designed for ~50 Salesforce Korea colleagues earlier this year. Same instinct, different form factor.
