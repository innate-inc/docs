# Contributing to the Innate docs

Thanks for helping make these docs better! Whether you're fixing a typo or writing a new guide, we're glad you're here.

## How to contribute

### Small fixes (typos, broken links, wrong commands)

1. Find the page on GitHub and click the pencil icon ("Edit this file")
2. Make your change and open a pull request

That's it — no local setup needed.

### Bigger changes (new pages, restructures)

1. Fork and clone this repository
2. Install the Mintlify CLI: `npm i -g mint`
3. Create a branch
4. Run `mint dev` from the repo root and preview at `http://localhost:3000`
5. Run `mint broken-links` before you push
6. Open a pull request

Not sure whether a change makes sense? Ask on [Discord](https://discord.com/invite/KtkyT97kc7) first — it can save you a rewrite.

## Writing guidelines

- **Lead with the action.** The first thing on a page should be what the reader does, not why the product is great.
- **Use active voice and "you".** "Run the command", not "the command should be run".
- **Show, don't just tell.** Every concept gets a code example or a screenshot.
- **One source of truth.** If a fact lives on two pages (version numbers, download links, setup steps), move it to `snippets/` and import it. Duplicated facts drift.
- **No "coming soon".** Only document what exists today. Roadmap promises go stale silently.
- **Test your commands.** If you write a shell command, run it on a robot (or in the simulator) first.
