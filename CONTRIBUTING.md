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

Readers skim. Every page should be as short as it can be while still getting them to the result.

**Page types.** Each page is one of these, never a mix:

| Type | Shape | Example |
| --- | --- | --- |
| How-to | One-sentence goal, numbered steps, how to check it worked | [Simulator setup](simulator/setup.mdx) |
| Concept | What it is, how it works (with a diagram), links onward | [How it works](software/overview.mdx) |
| Reference | One-line intro, a small example, then tables | [Movement API](software/skills/code-defined-skills/body-control-interfaces.mdx) |

**Structure.**
- Lead with what the reader does. No marketing.
- Show code first, explain after.
- Use a table for anything with two or more attributes: options, topics, commands, symptoms and fixes.
- Callouts are rare: at most one or two per page.
- Diagrams are images, never ASCII art. If you need one that doesn't exist yet, add a `<Callout icon="image" color="#7569FD">` that starts with **Image to make:** and describes it. Search for that phrase to find open requests.
- Say each fact once. Link to the page that owns it, or put it in `snippets/`.

**Plain English.**
- Aim for 15 words per sentence on average, and one idea per sentence.
- Use active voice, "you", and verbs that start steps: "Run", "Open", "Set".
- Prefer short, familiar words: *use* not *utilize*, *start* not *initiate*, *help* not *facilitate*, *to* not *in order to*, *if* not *in the event that*.
- Cut *simply*, *just*, *easily*, and sentences starting with *There is*.
- Use one term per concept. See the terminology list in `AGENTS.md`.

Further reading: [Diátaxis](https://diataxis.fr/), [Google developer style highlights](https://developers.google.com/style/highlights), [Microsoft top 10 tips](https://learn.microsoft.com/en-us/style-guide/top-10-tips-style-voice), [plain language guidelines](https://digital.gov/guides/plain-language/writing), and [Fowler's rules for plain English](https://www.ourdecline.com/english/plain.htm).

**No "coming soon", and test your commands** on a robot or in the simulator before you publish them.
