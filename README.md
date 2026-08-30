# Decision Advisor Skill

A structured decision-support skill for Codex-compatible agents. It uses first-principles framing, a small set of relevant mental models, alternative generation, red-team review, and an action-oriented recommendation.

## Trigger

The skill runs only when a user starts a message with one of these exact prefixes:

- `使用辅助决策skill：`
- `调用辅助决策skill：`

This keeps ordinary questions lightweight and makes deeper decision analysis an explicit choice.

## What It Produces

- A clear decision statement
- Facts, assumptions, unknowns, constraints, and ground truths
- Two to four relevant mental models
- Multiple options, including reversible or low-cost experiments
- A red-team and pre-mortem check of the leading option
- A recommendation with confidence, immediate actions, and review triggers

The included reference library covers 30 reusable mental models across decision-making, strategy, risk, uncertainty, planning, systems, and cognitive bias.

## Install In Codex

```powershell
python C:\Users\<you>\.codex\skills\.system\skill-installer\scripts\install-skill-from-github.py `
  --repo hubinhobby123-wq/decision-advisor-skill `
  --path skills/decision-advisor
```

Restart the Codex conversation after installation so the skill can be discovered.

## License

[MIT](LICENSE)
