# This starter vs a document-chat app (AnythingLLM)

AnythingLLM is a capable open-source app for chatting with your documents.
This starter is for a different job. Both are worth understanding before you
pick.

## What you are actually choosing

| Question | Document-chat app (AnythingLLM) | Kortix (this starter) |
|---|---|---|
| Primary job | Ask questions of documents in a chat window | Run agents that finish work and land it as a reviewable change |
| Where work lands | The chat reply | A change request against a git repo you own |
| Where config lives | The app's database/settings | Text files in one git repo |
| Runs on | Your machine or server, as a document app | Isolated sandbox per session, on any model |
| Permissions | App-level | Per-resource, per tool call (allow / ask / block) |
| Model choice | Bring your own key | Any model, per agent / session / message; your keys |
| Licence | Open source | Open source |

## When a document-chat app is the right call

If your need is genuinely "ask my notes a question," a document-chat app is
lighter and does that well. You do not need an operating system to read a PDF.

## When this starter is the right call

Pick the agent shape when the answer has to *do* something: patch the runbook,
open the ticket, reconcile the ledger, draft and queue the reply. That means
the agent must run where your systems are, hold scoped credentials, and commit
its result back for review — which is exactly what Kortix gives you.

The difference is ownership. AnythingLLM keeps your documents in its store;
Kortix keeps the whole company — agents, skills, memory, connectors — as files
in a git repo you own, so you can diff any change and roll any part back.

## Try it

Clone this repo, follow `docs/setup.md`, and run one real job end to end.
The full head-to-head is at
[anythingllm-alternative.com/kortix-vs-anythingllm](https://anythingllm-alternative.com/kortix-vs-anythingllm).
