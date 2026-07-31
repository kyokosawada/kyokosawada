# Giusippi Apa

**AI-forward engineer.** Retrieval, agent workflows, and the reliability work that makes them trustworthy.

[Portfolio](https://portfolio-apa.vercel.app/) · [Email](mailto:giusippi.apaii@gmail.com) · Manila, Philippines

---

Most of my work sits in one place: getting language models to do real work reliably, and proving it when they don't.

That means production systems where a model is one component among validators, retries, review queues and reconciliation — not the whole answer. The interesting engineering is almost never the prompt. It is what happens when the output is wrong, stale, or unavailable, and how anyone finds out.

Claude Code has been my daily driver since January 2026. Not a demo — it is how the work gets written, reviewed and shipped. Isolated branches, one task at a time, an explicit review pass, and my own read before anything lands.

If a system cannot cite the source it answered from, it should decline. I build the decline path first.

---

## Selected work

**UpRank** — *current work, private*
Local-SEO and lead-management platform. Around thirty scheduled jobs in production across operations, marketing and reporting. The generated-content pipeline is the part worth talking about: validators reject a bad draft, the retry carries the rejection reason into the next attempt, anything still failing is held for a human rather than published, and a daily reconcile records what actually happened instead of what we assumed.

**[rag-coach](https://github.com/kyokosawada/rag-coach)** — TypeScript
Retrieval-grounded assistant that refuses questions outside its corpus rather than guessing. The refusal is the feature; most of the work went into deciding when retrieved context genuinely supports an answer and when it only looks like it does.

**[gemini-slack-assistant](https://github.com/kyokosawada/gemini-slack-assistant)** — TypeScript
A chat-driven agent that reasons over a request and then acts — reading and sending against Gmail and Calendar, from Slack. Socket Mode, so it holds a live connection rather than polling.

**[lead-approval-bot](https://github.com/kyokosawada/lead-approval-bot)** — TypeScript
An inbound lead becomes an Approve / Deny card in Slack, and the decision sends the reply email. Built around a real constraint: the person deciding is on their phone, so it has to be one tap and the audit trail has to survive it.

---

## Stack

**Working in** — TypeScript · Python · Next.js · FastAPI · Node · Postgres / Supabase
**Models and tooling** — Claude · Gemini · retrieval pipelines · scheduled workers · Vercel
**Also shipped** — Java / Spring Boot · Kotlin · Go · Angular

---

<sub>BS Computer Science, De La Salle University</sub>
