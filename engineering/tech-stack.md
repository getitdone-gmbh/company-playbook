# Bevorzugter Tech-Stack

Gemeinsame Technologie über alle Produkte – damit Lösungen schneller entstehen, Wissen wiederverwendbar
bleibt und der 80/20-Grundsatz trägt: **80 % Standard-Stack, projektspezifisch nur, wo es wirklich nötig ist.**

## Frontend

**Next.js (App Router) + TypeScript + Tailwind + shadcn/Radix.**

- UI-Bausteine aus der gemeinsamen Bibliothek **`@getitdone-gmbh/component-library-react`** (library-first –
  Primitives nicht neu bauen), gestylt über die Design-Tokens **`@getitdone-gmbh/figma-design-tokens`**
  (Tailwind-Preset + CSS-Variablen, Light/Dark). Siehe [Design & Marken-Tokens](../design/README.md).
- Mehrsprachigkeit über `next-intl`. Icons aus einer Icon-Lib (Lucide), kein Inline-SVG.
- Deploy: Vercel.

## Backend

**NestJS + Prisma (PostgreSQL).**

- **Auth:** Passport-JWT mit getrennten Access-/Refresh-Secrets, `argon2`-Hashing; OAuth (Google/GitHub);
  API-Keys für Maschinenzugriff. **RBAC** über `@Roles()` + `RolesGuard`, secure-by-default.
- **Validierung:** `class-validator`-DTOs mit global registriertem `ValidationPipe`.
- **API-Doku:** Swagger/OpenAPI. **Async/Jobs:** Bull + Redis. **Security:** helmet, Throttler.
- **Config/Secrets:** `@nestjs/config` mit validiertem Schema; Secrets zentral über Infisical, nie im Code.
- **Health:** Terminus (`/health`, `/live`, `/ready`). **Tests:** Jest (Unit) + supertest (e2e, Wegwerf-DB);
  CI prüft lint + test + build vor dem Deploy.

## Referenz-Repositories

| Repo | Rolle |
|---|---|
| `component-library-react` | UI-Komponenten (shadcn/Radix) |
| `figma-design-tokens` | Design-Tokens (Single Source of Truth) |
| `cv-manager-api` | Backend-Bausteine (NestJS-Konventionen, Auth, DTOs, Swagger) — nutzt Mongoose; Konventionen übernehmen, Datenschicht auf Prisma |

Die verbindlichen Detail-Standards (inkl. der Fixes gegenüber Alt-Mustern) pflegen wir in den
Engineering-Stack-Definitionen der Entwicklungsumgebung; dieses Playbook hält die Richtung fest.
