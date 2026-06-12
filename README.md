# Innate Docs

Source for [docs.innate.bot](https://docs.innate.bot) — the developer documentation for MARS and Innate OS. This is where we explain how to drive the robot, build agents, write skills, and train manipulation policies.

Built with [Mintlify](https://mintlify.com). Pages are MDX files; navigation lives in `docs.json`.

## Run the docs locally

```bash
npm i -g mint
mint dev
```

Then open `http://localhost:3000`. Run `mint dev` from the repo root (next to `docs.json`).

Before opening a PR, check for broken links:

```bash
mint broken-links
```

## Repo layout

- `get-started/` — unboxing-to-first-command guides
- `robots/` — MARS hardware and the controller app
- `software/` — the Agent SDK: agents, skills, inputs, plus ROS2 reference
- `training/` — recording demonstrations and training ACT policies
- `snippets/` — shared content imported by multiple pages (version numbers, download links, warnings). **If a fact appears on more than one page, it belongs here.**

## Publishing

Merges to `main` deploy to production automatically via the Mintlify GitHub app.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Found a problem but don't want to fix it yourself? Tell us on [Discord](https://discord.com/invite/KtkyT97kc7).
