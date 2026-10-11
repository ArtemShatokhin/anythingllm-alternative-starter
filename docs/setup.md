# Run this starter on Kortix

Kortix is the open-source AI Operating System. This template is a company
knowledge agent: it answers from your files and lands the follow-up work as a
change request.

Time: about 10 minutes, no laptop setup.

## 1. Get the files into a repo you own

Fork this repo, or copy `agents/`, `kortix.yaml` and `docs/` into an existing
Kortix project. The repo *is* the company — agents, skills, memory and
connector config are all text files here.

## 2. Edit the manifest

Open `kortix.yaml`. Set the connectors you want the agent to reach (start with
`github` and `slack`). Leave `permissions.default: ask` until you trust the
agent's tool calls; then move a specific tool to `allow`.

## 3. Describe your company

Open `agents/company-knowledge.md` and replace the placeholder jobs with the
ones you actually want owned. Be concrete: "answers policy questions from
`docs/policies/`" beats "helps with knowledge".

## 4. Connect your sources

Point Kortix at the folders and tools that hold your knowledge. Connector
credentials are brokered server-side and never enter the machine, so the
agent reaches Slack or your ticket tracker without you pasting keys into a
config.

## 5. Start a session

Start a session against the repo — from the web app, Slack, the CLI, or the
API. It boots an agent on its own isolated Linux machine with your repo and
tools already on it. Watch it work live, then read its change request as a
diff before you merge.

## 6. Give it a schedule

Once it is doing a job reliably, add a trigger (a cron schedule or a signed
webhook) so the work starts with nobody asking. Review the change requests it
opens.

## Where to go next

- Product docs: https://kortix.com/docs
- The comparison with a document-chat app:
  https://anythingllm-alternative.com/kortix-vs-anythingllm
