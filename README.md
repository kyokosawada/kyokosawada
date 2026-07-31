<h1 align="center">Giusippi Apa</h1>

<p align="center">
  <b>AI-forward engineer.</b> I build software <i>with</i> agents, and I build the systems that keep them honest.
</p>

<p align="center">
  <a href="https://portfolio-apa.vercel.app/">Portfolio</a> ·
  <a href="mailto:giusippi.apaii@gmail.com">Email</a> ·
  Manila, Philippines
</p>

---

Most of my work now sits in one place: **getting language models to do real work reliably, and proving it when they don't.**

Day to day that means production systems where a model is one component among validators, retries, review queues and reconciliation - not the whole answer. The interesting engineering is almost never the prompt. It is what happens when the output is wrong, stale, or unavailable, and how anyone finds out.

### How I work

- **Claude Code as a daily driver since January 2026.** Not a demo - it is how the work gets written, reviewed and shipped.
- **Agents supervised, not trusted.** Isolated worktrees, one task per agent, an explicit review pass, and a human gate before anything lands.
- **Grounded answers or none.** If a system can't cite the source it answered from, it should decline. I build the decline path first.
- **Scheduled work over manual work.** Currently ~30 scheduled jobs in production across operations, marketing and reporting.

---

## Selected work

### [firstmate](https://github.com/kyokosawada/firstmate) · Shell
An agent fleet you talk to through one interface. Spawns coding agents into isolated worktrees, supervises them, and refuses to tear down work that has not landed.

The whole design question is *what an agent is not allowed to do*: it cannot merge without a human word, cannot discard uncommitted work, and cannot report a task complete without evidence. Multi-runtime, with the safety boundaries in one place rather than scattered through prompts.

### [rag-coach](https://github.com/kyokosawada/rag-coach) · TypeScript
Retrieval-grounded assistant that **refuses questions outside its corpus** rather than guessing at them.

The refusal is the feature. An assistant that answers everything is indistinguishable from one that answers nothing correctly, and the failure is silent - which makes it the expensive kind.

### [orban-labs-challenge](https://github.com/kyokosawada/orban-labs-challenge) · Python · FastAPI
Two services built to a brief in a fixed window: a notes API with search, and a URL shortener with expiry, click analytics and destination validation. Test-first, incremental commits, with the AI usage disclosed in the repo rather than hidden.

### [gemini-slack-assistant](https://github.com/kyokosawada/gemini-slack-assistant) · TypeScript
A chat-driven agent that reasons over a request and then *acts* - reading and sending against Gmail and Calendar from Slack. Socket Mode, so it holds a live connection rather than polling.

---

## Stack

**Working in:** TypeScript · Python · Next.js · FastAPI · Node · Postgres / Supabase
**Also shipped:** Java / Spring Boot · Kotlin · Go · Angular
**Models & tooling:** Claude · Gemini · retrieval pipelines · scheduled workers · Vercel

---

<sub>BS Computer Science, De La Salle University. Currently building lead-management and local-SEO automation.</sub>
