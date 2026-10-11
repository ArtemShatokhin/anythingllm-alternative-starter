# AnythingLLM alternative starter — an open-source company knowledge agent on Kortix

An open-source, self-hosted starting point for a team that has outgrown a
document-chat app and wants a **company knowledge agent** — one that reads the
same files, remembers what it learned, and puts the result where the work
already lives.

This template runs on **[Kortix](https://kortix.com)** — the open-source AI
Operating System. In Kortix your agents, skills, company memory and connectors
are text files in one git repo you own, on any model with your own keys,
self-hosted or on managed cloud. Every session runs on its own isolated
computer and lands its work as a change request you review and merge.

The template is small on purpose: an agent file, a skill, a manifest and the
docs. Adapt the files, point Kortix at your repo, and the agent inherits your
conversation history as memory.

## Why a starter, not a chatbot

AnythingLLM is a strong document-chat app: you point it at files and ask
questions. A **company knowledge agent** is a different shape of tool. The
question is not *"can it search my documents"* but *"can the answer leave the
chat window and change something"* — open the ticket, update the runbook,
draft the reply. That needs the agent to run where your systems are, with
scoped permissions, and to commit its work back as a reviewable change.

Kortix is built for that second shape, and it is open source, so the harness,
the skills and the memory are files you can read and roll back.

See the full comparison at
[anythingllm-alternative.com/kortix-vs-anythingllm](https://anythingllm-alternative.com/kortix-vs-anythingllm).

## What's in the repo

```
kortix.yaml                 the manifest: image, connectors, triggers
agents/company-knowledge.md the agent: instructions + which tools it may touch
docs/setup.md               run it on Kortix in ~10 minutes
docs/vs-anythingllm.md      where a document-chat app stops and this starts
docs/faq.md                 licence, models, self-hosting, data residency
```

## Quick start

1. Fork or clone this repo, or copy the files into an existing Kortix project.
2. Connect your sources (a docs folder, a wiki, a ticket tracker) — see
   `docs/setup.md`.
3. Edit `agents/company-knowledge.md` to describe your company and the jobs
   the agent owns.
4. Start a session. It runs on its own machine, reads your repo, and opens a
   change request with the work it did.

## Learn more

- Kortix on the web: https://kortix.com
- Product docs: https://kortix.com/docs
- Kortix on GitHub: https://github.com/kortix-ai/suna
- The campaign site: https://anythingllm-alternative.com
