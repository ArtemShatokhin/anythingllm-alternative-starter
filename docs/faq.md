# FAQ

**Is Kortix open source?**
Yes. Kortix is the open-source AI Operating System. Your agents, skills,
memory and connectors are text files in one git repo you own, and the harness
is open source too.

**Do I have to self-host it?**
No. Self-host, run it in your own VPC or on-prem, or use managed cloud. The
same repo works in all three.

**Which models can I use?**
Any. Pick the model per agent, per session or per message — Anthropic, OpenAI,
Google, or any OpenAI-compatible endpoint — with your own keys, or the ChatGPT
subscription you already pay for. Kortix is model-agnostic so you can switch
the day a better model lands.

**Is this a chatbot?**
No. It is a company knowledge *agent*. It answers from your files and then
lands the follow-up work as a change request you review and merge.

**How is this different from AnythingLLM?**
AnythingLLM is a document-chat app: you ask it questions. Kortix is an
operating system for agents that finish work and commit it back to a repo you
own. See `docs/vs-anythingllm.md`.

**Is it safe to let it act?**
Every tool call is ruleable — allow, ask, or block — down to the arguments it
was given. Default is deny for agents, session work lands as a change request,
and connector credentials are brokered server-side and never enter the machine.

**How do I start?**
Follow `docs/setup.md`. About ten minutes, no laptop setup.

**Where are the docs?**
https://kortix.com/docs
