# Documentation project instructions

This is the Mintlify docs site for the Innate robotics platform (MARS robot, Innate OS, Agent SDK), deployed at docs.innate.bot.

- Pages are MDX files with YAML frontmatter
- Navigation and redirects live in `docs.json` — every new page must be added there
- Run `mint dev` to preview locally, `mint broken-links` to check links
- Shared content (version numbers, download links, repeated warnings) lives in `snippets/` and is imported with `import ... from "/snippets/..."` — never duplicate these facts inline

## Terminology

- "MARS" (all caps) — the robot. Not "Mars".
- "Innate OS" — the robot's operating system
- "agent" — a high-level behavior program (a Python class extending `Agent`)
- "skill" — a robot capability; either **code-defined** (Python) or **policy-defined** (trained ACT checkpoint)
- "input" / "input device" — a data source feeding the agent (e.g. microphone)
- "leader arm" — the small teleoperation controller arm that ships with MARS
- "controller app" — the Innate Controller App (Android/iOS)

## Style preferences

- Use active voice and second person ("you")
- Lead with the action; keep marketing language out of doc pages
- Use sentence case for headings
- Bold for UI elements: tap **Configuration** -> **Mapping**
- Code formatting for file names, commands, paths, and code references
- No "coming soon" or undated roadmap promises — document only what ships today

## Content boundaries

- Don't document internal Innate infrastructure (cloud deployment, CI)
- Hardware fixes for specific robot batches go under `robots/mars/troubleshooting/`, linked from the Troubleshooting page — not in the main navigation
