These are Lauren Tan's pstack skills: playbooks, investigation, verification, code review, and the engineering principles she uses day to day. This unofficial mirror brings them into bb without rewriting them, and keeps them current.

## What you get

- **All of pstack, as slash commands.** Start with `/poteto-mode`: it picks one of Lauren's 23 playbooks and runs the other skills its steps need. `/poteto-help` points you to the right skill for a task.
- **On by default, or only where you want it.** Turn pstack on for every project, or leave the default off and turn it on in the projects you pick. Each project can also switch individual skills.
- **Nothing breaks when you turn skills off.** Skills that other active skills need stay on, and the page shows which skill uses them. Turning one off for real asks first and tells you exactly what else goes with it.
- **A Start here card** with Lauren's recommended first steps, which you can close for good.

## How it stays current

A GitHub Actions job checks [cursor/plugins](https://github.com/cursor/plugins/tree/main/pstack) every day. When pstack changes, it copies her files unchanged, validates them, and publishes a new plugin release. Changes to executable helper scripts, or anything that fails a check, wait for a human review instead. The page shows the bundled pstack version and commit, and tells you when a newer release exists. Update with `bb plugin update pstack-for-bb`.

## Compatibility with bb

pstack was written for Cursor. Two skill names are normalized so bb can find them, and one helper script is adjusted so it never marks a bb worktree as safe to delete. Every change is listed in the [compatibility notes](https://github.com/erikmackinnon/bb-plugin-pstack-for-bb/blob/main/compat/README.md). A short note tells agents how Cursor terms map to bb tools.

## Requirements

bb 0.45 or newer, an agent provider, and npm for the Git install. Some skills use extra tools such as Bun or GitHub CLI, and the page flags them. Multi-model skills work best with more than one provider installed. Update checks contact GitHub. No account or API key is needed.

## Attribution

**Skills © 2026 Lauren Tan, MIT**, from [cursor/plugins](https://github.com/cursor/plugins/tree/main/pstack). Plugin code © 2026 Erik MacKinnon, MIT. Not affiliated with or endorsed by Lauren Tan, Cursor, or bb.
