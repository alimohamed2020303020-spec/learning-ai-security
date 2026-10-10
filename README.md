# Learning AI Security 

My notes while learning AI security from scratch.
I'm a beginner who also learns Python and C++, and I
write here what I try, what fails, and what I learn.

## What's inside

### Agent Breaker (by Lakera)
Agent Breaker is a practice game where you attack AI
agents that use tools. In these levels, I attacked a
chat app that connects to a weather tool (MCP).

| Level | Difficulty | Goal | Result |
|-------|-----------|------|--------|
| [Level 1](agent-breaker/level-1.md) | Novice | Leak the user's email | 100/100 |
| [Level 2](agent-breaker/level-2.md) | Adept | Leak the full chat history | 100/100 |
| [Level 3](agent-breaker/level-3.md) | Master | Leak the full chat history (hardened app) | 98/100 |
| [Level 4](agent-breaker/level-4.md) | Expert | Leak the full chat history (extra filter) | 98/100 |

Each file has the objective, my approach, what I
learned, and ideas for defense.

## Main lessons so far
- **Tool poisoning:** text inside a tool description can
  work like a command for the model.
- **Read the objective again at every level.** It can
  change.
- **Probe first, then expand:** small tests, one change
  at a time.
- **Defense needs layers outside the model:** least
  privilege, validating tool calls in code, and treating
  third-party tool descriptions as untrusted.
- **Filters that block instructions can miss examples that teach the same behavior.**

## Note
All attacks here were done inside Lakera's Agent Breaker,
a legal practice environment made for this. I don't
publish full attack prompts, I write about the ideas and
what I learned.

More notes will be added as I learn.
