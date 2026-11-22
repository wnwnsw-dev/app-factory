# Technologies

## Now (v0 example)
- Targets: iOS, Android, web — Expo
- Language: TypeScript
- Navigation: Expo Router
- Styling: NativeWind (Tailwind)
- Storage: Expo SQLite (local only)
- State: React state
- Storybook: stories for UI components
- Tests: Jest + React Native Testing Library

## Modes
- One app; `APP_MODE` chooses the data adapter at build time
- `mockup` → `*.mockup.ts` (dummy data); `production` → `*.production.ts` (SQLite)
- Alias lives in `metro.config.js`; production bundle excludes dummy code

## Later (factory defaults, not used in this example)
- Supabase + Drizzle ORM
- Supabase Auth behind AuthProvider
- Zod, Sentry, Maestro
- EAS + GitHub Actions
