---
name: gdoc
description: Write, edit, and review technical documentation that follows the Google developer documentation style guide (https://developers.google.com/style). Use this skill whenever the user asks to write developer docs, READMEs, API references, tutorials, how-to guides, release notes, error messages, UI text, or code comments — or to review, edit, lint, or rewrite any technical content "in Google style", "per the style guide", or "for docs". Also use it when the user asks style questions like "should this be hyphenated", "sentence case or title case", "can I say whitelist", or "how do I write this procedure".
---

# Google developer documentation style

This skill distills the Google developer documentation style guide
(https://developers.google.com/style) into rules Claude can apply when writing,
editing, or reviewing technical documentation. The guide's content is licensed
under CC BY 4.0; attribute the guide when quoting it.

The guide's own philosophy: these are guidelines, not laws. Break a rule when
doing so makes the content clearer for the reader — but be consistent within a
document. Reference hierarchy when a question isn't answered here:
(1) the project's own style rules, (2) this guide, (3) Merriam-Webster for
spelling, Chicago Manual of Style for general style, Microsoft Writing Style
Guide for technical style.

## Workflow

1. **Writing new docs**: Apply the core rules below. Read the reference file
   for each content type you produce (procedures → `references/formatting-organization.md`,
   code → `references/computer-interfaces.md`, and so on).
2. **Editing or reviewing docs**: Check the text against the core rules first,
   then scan `references/word-list.md` for banned or preferred terms, then read
   the category references relevant to the problems you find. Report issues
   with the rule and a suggested fix, not just a flag.
3. **Answering a style question**: Find the topic in the category map below,
   read that reference file, and answer with the rule plus an example. If the
   answer might have changed or the term isn't covered, fetch the live page —
   every rule below lists its source URL.

## Core rules (the "highlights")

Voice and tone:
- Be conversational, friendly, and respectful — a knowledgeable friend, not a
  marketer or a lecturer. Not frivolous, not formal. Don't use "please" in
  instructions or link introductions. Don't pre-announce features or make
  promises about the future.
- Use second person ("you"), not "we". Use active voice: make clear who acts.
- Use present tense. Avoid "will" except for true future events.
- Contractions like "it's", "don't", "you're" are encouraged. Avoid "let's",
  "please note", "at this time", exclamation marks, pop-culture references,
  internet slang (tl;dr), and starting every sentence the same way.
- Be prescriptive: recommend one path to the goal rather than listing options.
  No superlatives or unverifiable claims ("fastest", "guaranteed", "prevents
  attacks" — write "helps prevent", "is designed for security", and cite
  sources for performance numbers).

Language:
- Use standard American spelling (Merriam-Webster, first-listed form).
- Put conditions before instructions: "To delete the file, click Delete" and
  "If you want X, do Y" — not the reverse. The reader should know whether a
  step applies before reading how to do it.
- Word choice for requirements: *must* = required; *can* = optional or
  permission; *might* = possible outcome; "We recommend" = recommendation.
  Avoid *should* (ambiguous), *may*, *could*, *would*, *shall*. Never "the
  value should be true" — say who sets it or what to do if it isn't.
- Keep helper words that casual English drops: *that*, *then*, *of*, articles,
  relative pronouns ("If X, then Y", "assumes that you have", "and then run").
  Qualify code keywords with a noun ("the `example.yaml` file"). No more than
  two nouns stacked as modifiers. Place *only* directly before what it limits.
- Don't use figurative, idiomatic, culturally specific, gendered, ableist, or
  violent language. No humor, no seasons as dates. Use singular "they". Jargon:
  write around it, replace it, or define it on first use (in parentheses or by
  a link). See `references/word-list.md`.

Formatting:
- Sentence case for all titles and headings ("Create a service account",
  not "Create a Service Account").
- **Bold** only for UI elements and run-in headings. *Italics* for defining
  terms, words-as-words, math variables, and titles of full-length works.
  `Code font` for code, filenames, commands, HTTP status codes, placeholders.
  Never underline (that's for links). Never use ampersand for "and" in text.
- Serial (Oxford) commas. Numbered lists for sequences, bulleted lists for
  unordered sets, description lists for term–definition pairs.
- Placeholders: all caps with underscore delimiters, in code font, e.g.
  `PROJECT_ID`. Explain each placeholder after the code block ("Replace
  PROJECT_ID with ...").
- Unambiguous dates: "January 19, 2017", never "1/19/2017". Times: "9:00 AM".

Linking:
- Descriptive link text — the link is the title or a description of the
  target. Never "click here" or "this document". Standard cross-reference
  form: "For more information, see [Title of page]."

Accessibility and global audience:
- Provide alt text for images. Don't rely on color, direction ("left menu",
  "above"), or device-specific gestures to convey meaning.
- Write short, simple sentences that translate well. Include "that" and
  "then" helper words. Define jargon and abbreviations on first use.

Timelessness:
- Avoid "currently", "now", "soon", "new", "as of this writing", "eventually",
  "in the future". State facts; give version numbers or dates when a time
  anchor is needed.

## Category map

Read the reference file before doing substantive work in its area. Each file
lists the source URL for every topic so you can fetch details on demand.

| Task or question | Read |
|---|---|
| Word choice, banned terms, spelling of specific terms | `references/word-list.md` |
| Tone, accessibility, inclusive language, jargon, global audience, timeless docs, claims, future features, third-party content | `references/general-principles.md` |
| Grammar: abbreviations, voice, tense, person, pronouns, articles, capitalization, contractions, plurals, possessives, prepositions, sentence structure, reference verbs | `references/language-grammar.md` |
| Punctuation: commas, colons, dashes, hyphens, ellipses, parentheses, periods, quotation marks, semicolons, slashes | `references/punctuation.md` |
| Structure: headings, lists, procedures, tables, notices, numbers, dates, units, examples, images, footnotes, paragraphs, math, phone numbers | `references/formatting-organization.md` |
| Links and cross-references | `references/linking.md` |
| Code in text, code samples, command-line syntax, placeholders, UI elements, API reference comments | `references/computer-interfaces.md` |
| HTML vs Markdown, semantic tagging, example domains and names, filenames, trademarks, product names | `references/html-naming.md` |

## Review checklist

When asked to review or lint a document, check in this order and report each
finding as: location → rule → suggested rewrite.

1. Headings: sentence case; unique; descriptive; no ampersands; no terminal periods.
2. Person and voice: "you" not "we"; active voice; present tense.
3. Conditions before instructions; one action per step; numbered steps.
4. Word list violations (whitelist/blacklist, master/slave, e.g./i.e., "click here",
   "please", "simply/easily/just", "allows you to", "in order to", and so on).
5. Formatting: bold only on UI elements; code font on code items; correct
   placeholder style; serial commas; en/em dash usage; unambiguous dates.
6. Links: descriptive text; "see" phrasing; punctuation outside link text.
7. Accessibility: alt text present; no directional or color-only references.
8. Timeless wording: no "currently/soon/new/will".

Do not "fix" text that quotes UI labels, code identifiers, or official product
names — match the source exactly, even when it violates a rule, and note that
you did so.
