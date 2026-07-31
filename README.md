<div align="center">

```
┌──────────────────────────────────────────────────────────────┐
│  giusippi apa                                                │
│  ai-forward engineer                                         │
│                                                              │
│  > retrieval, agent workflows, and the reliability work       │
│    that makes them trustworthy                               │
└──────────────────────────────────────────────────────────────┘
```

[![Portfolio](https://img.shields.io/badge/portfolio-portfolio--apa.vercel.app-14B8A6?style=for-the-badge&logoColor=white)](https://apa-dev.netlify.app/)
[![Email](https://img.shields.io/badge/email-giusippi.apaii@gmail.com-0f766e?style=for-the-badge&logoColor=white)](mailto:giusippi.apaii@gmail.com)

</div>

```console
$ whoami --verbose

Most of my work sits in one place: getting language models to do real
work reliably, and proving it when they don't.

Production systems where a model is one component among validators,
retries, review queues and reconciliation - not the whole answer.

The interesting engineering is almost never the prompt. It is what
happens when the output is wrong, stale, or unavailable, and how
anyone finds out.
```

```console
$ cat principles.txt

[1]  Claude Code as a daily driver since Jan 2026. Not a demo - it is
     how the work gets written, reviewed and shipped.

[2]  Isolated branches, one task at a time, an explicit review pass,
     and my own read before anything lands.

[3]  If a system cannot cite the source it answered from, it should
     decline. I build the decline path first.
```

```console
$ ls -la ./work

drwx------  UpRank                    current work, private
-rwxr-xr-x  rag-coach                 typescript
-rwxr-xr-x  gemini-slack-assistant    typescript
-rwxr-xr-x  lead-approval-bot         typescript
```

### `UpRank` &nbsp;<sub>current work · private</sub>

Local-SEO and lead-management platform. **~30 scheduled jobs in production** across operations, marketing and reporting.

The generated-content pipeline is the part worth talking about: validators reject a bad draft, the retry carries the rejection reason into the next attempt, anything still failing is held for a human rather than published, and a daily reconcile records what actually happened instead of what we assumed.

### [`rag-coach`](https://github.com/kyokosawada/rag-coach)

Retrieval-grounded assistant that **refuses questions outside its corpus** rather than guessing. The refusal is the feature - most of the work went into deciding when retrieved context genuinely supports an answer and when it only looks like it does.

### [`gemini-slack-assistant`](https://github.com/kyokosawada/gemini-slack-assistant)

A chat-driven agent that reasons over a request and then *acts* - reading and sending against Gmail and Calendar, from Slack. Socket Mode, so it holds a live connection rather than polling.

### [`lead-approval-bot`](https://github.com/kyokosawada/lead-approval-bot)

An inbound lead becomes an Approve / Deny card in Slack, and the decision sends the reply email. Built around a real constraint: the person deciding is on their phone, so it has to be one tap and the audit trail has to survive it.

```console
$ cat stack.json

{
  "working_in":       ["TypeScript", "Python", "Next.js", "FastAPI",
                       "Node", "Postgres/Supabase"],
  "models_tooling":   ["Claude", "Gemini", "retrieval pipelines",
                       "scheduled workers", "Vercel"],
  "also_shipped":     ["Java/Spring Boot", "Kotlin", "Go", "Angular"]
}
```

```console
$ tail -1 ~/.education
BS Computer Science, De La Salle University
```
