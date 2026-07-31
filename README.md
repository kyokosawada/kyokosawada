# Giusippi Apa

AI-forward engineer in Manila. I build software **with** agents, and I build the parts that keep them honest.

[Portfolio](https://portfolio-apa.vercel.app/) · [Email](mailto:giusippi.apaii@gmail.com)

## Now

**Building a store-visit assistant** — policy library in, checklist and a sourced print-ready report out, with actions carried forward between visits so follow-through is visible. Python.

**Running ~30 scheduled jobs in production** at UpRank across operations, marketing and reporting, and steadily converting the ones that need judgement from "a model wrote it" into "a model wrote it, a validator checked it, and a human saw the ones that failed."

**Living in Claude Code** since January 2026 — it is how the work gets written, reviewed and shipped, not something I tried once.

## What I actually care about

The interesting engineering is almost never the prompt.

It is what happens when the output is wrong, stale, or unavailable, and how anyone finds out. A model that is right 95% of the time and silent about the other 5% is worse than one that refuses, because nobody knows which answer they are holding.

So: validators before publishing, retries that carry the reason for the failure into the next attempt, a review queue for anything still failing, and a reconcile job that records what actually happened rather than what we assumed.

## Work

**UpRank** · *current, private* — local-SEO and lead-management platform. The generated-content pipeline is the piece I would talk about in an interview: it fails safely and says so.

**[rag-coach](https://github.com/kyokosawada/rag-coach)** — retrieval-grounded assistant that refuses questions outside its corpus rather than guessing. The refusal is the feature.

**[gemini-slack-assistant](https://github.com/kyokosawada/gemini-slack-assistant)** — an agent that reasons over a request and then *acts*, against Gmail and Calendar from Slack.

**[lead-approval-bot](https://github.com/kyokosawada/lead-approval-bot)** — inbound lead becomes an Approve / Deny card in Slack; the decision sends the reply email. One tap, because the person deciding is on their phone.

## Tools

TypeScript · Python · Next.js · FastAPI · Postgres / Supabase · Claude · Gemini
Previously: Java / Spring Boot · Kotlin · Go · Angular

---

<sub>BS Computer Science, De La Salle University · open to AI and automation engineering roles</sub>
