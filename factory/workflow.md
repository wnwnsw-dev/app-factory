# App workflow

Each new app is a copy of this factory in its own repository. For now, this repo's app lives in `example/`.

Repeat these steps per app. One step at a time: ask, get approval, write, stop.

## Steps
1. Context — `context.md`: purpose, fields to store, scope, success.
2. Technologies — `technologies.md`: what we use now vs factory defaults later.
3. Module — `modules/<module>/module.md`: goal, scope, journey list. You define it; I only ask.
4. Journey — one `journeys/<name>.md` per user journey: steps, states, mockup location.
5. Mockup — you build each journey in `example/app/` using `factory/agents/mockup.md`; mockup mode uses dummy data.
6. Todo + verification — `modules/<module>/todo.md` and `verify.md`. Approve before code.
7. Implement + test — one task at a time; tests must pass; you check `verify.md`. No auto-advance.
8. Extract — only what worked becomes a factory default.

## Rules
Minimum documents. No rule written twice. Never create a file without asking. Never move on without your tick.
After each step, append one line to `example/timeline.md`.
