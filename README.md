# Google developer documentation style skill

A Claude skill that writes, edits, and reviews technical documentation in the
[Google developer documentation style](https://developers.google.com/style).

## Install

**Claude Desktop:** Open **Settings > Capabilities > Skills**, then upload
`gdoc.skill`.

**Claude CLI (Claude Code):** Copy the `gdoc/` folder into your skills
directory:

```sh
cp -r gdoc ~/.claude/skills/gdoc
```

To scope the skill to a single project instead, copy it into that project's
`.claude/skills/` directory.

After you install the skill, ask Claude to write, review, or answer questions
about docs "in Google style."

## Attribution

This skill distills the Google developer documentation style guide, which
belongs to Google and is licensed under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). See
https://developers.google.com/style.
