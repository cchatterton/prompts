# Agent roles and task prompts

This repository holds reusable instructions for working with Codex. It has two parts:

- [`agents/`](agents/) defines the role or perspective: the **“act as”** part of a request.
- [`prompts/`](prompts/) defines the task or command: the **“please do”** part of a request.

Choose one agent and one prompt, then give Codex the material needed for the task. The prompt should be carried out through the chosen agent's perspective. The files are plain-language instructions, not programs.

## How to ask Codex

> Use `https://github.com/cchatterton/prompts`. Act as the agent in `agents/Strategist.md` and do `prompts/Review this URL.md` for [URL].

Or, for a transcript:

> Use `https://github.com/cchatterton/prompts`. Act as the agent in `agents/Personal Assistant.md` and do `prompts/Summarise this transcript.md` using the transcript below: [transcript].

You can refer to an agent or prompt by its filename when the choice is clear. Include a URL, transcript, document, or other input required by the chosen prompt.

## For Codex

When asked to use this repository:

1. Read the full text of the requested file in `agents/` and the requested file in `prompts/` from the current repository version.
2. Use the agent file to set the role, priorities, and perspective. Use the prompt file to determine the task and required output.
3. Apply both sets of instructions to the user's supplied material. Follow any more specific directions in the user's request.
4. If a requested file or required input is missing or ambiguous, ask for the missing detail.

The agent answers **“as whom?”** and the prompt answers **“do what?”**. The same prompt can produce different useful results with different agents.
