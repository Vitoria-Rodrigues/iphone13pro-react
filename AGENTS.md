# iPhone 13 Pro React Agents Context

This document serves as the sovereign root context router (Layer 1) for AI agents operating in the `Vitoria-Rodrigues/iphone13pro-react` repository.

## Navigation

- [README.md](./README.md): Primary developer documentation, architecture overview, and pnpm setup guide.
- [.agents/plugins.json](./.agents/plugins.json): Antigravity plugin registry importing domain plugins from `@vitoria-rodrigues/agent-mesh`.
- [pnpm-workspace.yaml](./pnpm-workspace.yaml): Centralized dependency catalogs (`catalogMode: strict`) and `@vitoria-rodrigues/agent-mesh` registration.
- [package.json](./package.json): Scoped package manifest (`@vitoria-rodrigues/iphone13pro-react`) and Vite scripts.

## Architecture

The application is an interactive React 19 and Vite 7 frontend SPA replicating the Apple iPhone 13 Pro product showcase with dynamic finish selection and responsive layout:

- **`src/pages/Home.jsx`**: Main product landing page coordinating navigation, promotional banner, and interactive color-selection state.
- **`src/components/`**: Modular UI components (`Header.jsx`, `NaviPhone.jsx`, `PromoBanner.jsx`, `Button.jsx`, `Card.jsx`) paired with dedicated component CSS stylesheets.
- **`src/assets/img/`**: Static product images for each iPhone 13 Pro finish (`iphone_blue.jpg`, `iphone_golden.jpg`, `iphone_graphite.jpg`, `iphone_green.jpg`, `iphone_silver.jpg`) and `logo_apple.svg`.
- **Hosting**: Continuous deployment via Vercel (`https://iphone13-pro-react.vercel.app/`).

## Scoped Guardrails

- MUST maintain a strict senior, objective, and technical tone across all communications, documentation, and code.
- MUST conduct conversational chat responses in Brazilian Portuguese (pt-BR) while keeping all code, configuration files, commit messages, and technical documentation in English (en-US).
- MUST NOT use emojis anywhere in code, markdown headers, body text, commit messages, or chat responses (Zero-Emoji Invariant).
- MUST use `pnpm` exclusively and consume all dependencies via `catalog:` entries in `pnpm-workspace.yaml` (never raw semver strings in `package.json`).
- MUST consume `@vitoria-rodrigues/agent-mesh` solely via `catalog:plugins-stack` and `.agents/plugins.json` without duplicating local skills or rules inside `.agents/`.
- MUST use Conventional Commits v1.0.0 (`<type>(<scope>): <description>`) and sign commits with SSH (`git commit -S -m "..."`) when `user.signingkey` is configured.
- MUST use relative paths for all Markdown links inside repository files.

## Required Skills

When operating in this repository, agents MUST activate the relevant `@vitoria-rodrigues/agent-mesh` skill:

- **`router-architect`**: Active when authoring or auditing `AGENTS.md` context routers.
- **`readme-architect`**: Active when updating or auditing `README.md` documentation.
- **`monorepo-architect`**: Active when auditing `pnpm-workspace.yaml` catalogs or `package.json` manifests.
- **`github-flow-operator`**: Active when creating branches, commits, or pull requests.
- **`browser-auditor`**: Active when visually inspecting the live Vite or Vercel UI.
