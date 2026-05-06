# foresight-institute-agents

Constitution, skills, and operational components for AI agents serving Foresight Institute's mission.

## About

Foresight Institute works toward beneficial long-term futures across AI safety, longevity, neurotechnology, molecular machines, and computer security. As AI agents become part of how the Institute operates, researches, and communicates, those agents need a shared foundation — a clear articulation of the values they should embody and a library of capabilities they can draw on.

This repository is that foundation. It contains:

- **A constitution** — a system prompt encoding Foresight Institute's values, commitments, and operating principles, intended to be loaded by any AI agent acting on the Institute's behalf.
- **Skills** — reusable, composable agent capabilities following the agent skills protocol, enabling agents to handle specific tasks consistently and well.

Both are openly licensed. Other organizations working on value-aligned AI agents are encouraged to fork, adapt, and contribute back.

## Repository Structure

```
.
├── constitution/       # System prompt and supporting documentation
├── skills/             # Agent skills, each in its own subdirectory
│   └── <skill-name>/
│       └── SKILL.md
├── LICENSE             # Apache License 2.0
└── README.md
```

## The Constitution

The constitution articulates:

- Foresight Institute's mission and the disposition agents should bring to it
- Values and commitments that guide agent behavior
- Operating principles for handling ambiguity, disagreement, and edge cases
- Boundaries — what agents should not do, regardless of instructions

It is intentionally a living document. As our understanding of agentic systems matures, so will the text.

## Skills

Skills follow the agent skills protocol: each skill is a directory containing a `SKILL.md` file with progressive disclosure — a short description that helps the agent decide when to invoke the skill, and detailed instructions loaded on demand. Skills may include supporting scripts, templates, or reference data alongside the markdown.

## Usage

To use this repository in your agent:

1. Load the constitution as the agent's system prompt, or merge it with your existing prompt.
2. Make the `skills/` directory available to the agent. The exact mechanism depends on your runtime — consult your agent framework's documentation for loading skills.

A reference integration will be added as the project matures.

## Contributing

Substantive changes to the constitution — those affecting values, commitments, or operating principles — are reviewed by Foresight Institute and should be opened as pull requests with a written rationale. Editorial improvements and clarifications are welcome from anyone.

New skills should be self-contained, well-documented, and address tasks Foresight agents are likely to encounter. Open an issue first if you are unsure whether a proposed skill fits the repository's scope.

## License

This project is licensed under the Apache License 2.0 — see the [LICENSE](./LICENSE) file for details.
