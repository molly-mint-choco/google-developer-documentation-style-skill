# Linking

Condensed from the "Linking" category of the Google developer documentation
style guide (CC BY 4.0).

## Cross-references and linking
https://developers.google.com/style/cross-references

- Link text must describe the target. Best: the exact title or heading of the
  target, capitalized as the target capitalizes it. Acceptable: a noun-phrase
  description of the target.
- Never use "click here", "this page", "here", a bare "link", or a raw URL as
  link text in prose. (Raw URLs are OK in code font when the URL itself is
  the content, such as an API endpoint.)
- Standard formula for a pointer elsewhere:
  "For more information, see [Title]." — and use "about X" rather than
  "on X" when adding a topic: "For more information about indexes, see ...".
- Tell the reader when a link leaves the current context or downloads a file.
- Put punctuation and quotation marks outside the link text. Don't italicize
  or quote titles when they are the link text.
- Link the first mention of a concept per page; don't relink the same target
  repeatedly. Don't stack many links in one sentence.
- Prefer linking to canonical, stable targets; avoid deep links likely to rot.
- Don't make a cross-reference the only path to information the reader needs
  right now — inline the essential fact and link for depth.

## Headings as link targets
https://developers.google.com/style/headings-targets

- Give important headings explicit, stable anchor IDs so inbound links don't
  break when the heading text changes.
- Anchor style: lowercase, hyphen-separated words (dash-case), descriptive
  and unique on the page.
- When you change heading text, keep the old ID or add a redirect anchor.
