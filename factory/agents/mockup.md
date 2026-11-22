# Mockup agent

Read only these files, in order. Do not scan the repo:
1. `factory/agents/mockup.md` (this file)
2. `example/context.md`
3. `example/technologies.md`
4. `example/modules/<module>/module.md` (one module)
5. The one journey file named in the task
6. `example/app/theme/tokens.ts` (create if missing)
7. `example/app/components/index.ts` (create if missing)
8. `example/timeline.md` (match format; append after the last line)

Build that journey into `example/app/` only. Never create a separate mockup folder.

## Rules
- Expo + TypeScript + Expo Router + NativeWind.
- Dummy data in `data/series-repository.mockup.ts`; add `data/series-repository.production.ts` as a stub. `APP_MODE` alias selects one in `metro.config.js`.
- Implement only the steps and states in the journey file.
- All colors, spacing, and type in `theme/tokens.ts`. No hard-coded values in screens.
- One Storybook story per UI component, using those tokens. Production reuses them.
- Reuse existing components; add to them. No docs, tests, CI, or extra config except the timeline line.
- When the prototype runs, append one line to `example/timeline.md`: next number — Mockup: <journey> → files touched. Change nothing else.
- Stop when it runs; report file list + start command.
