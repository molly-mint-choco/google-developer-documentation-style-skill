# Punctuation

Condensed from the "Punctuation" category of the Google developer
documentation style guide (CC BY 4.0). Each section lists its source URL.

## Commas
https://developers.google.com/style/commas

- Always use the serial (Oxford) comma: "a, b, and c".
- Comma after introductory phrases and conditions: "After the build finishes,
  deploy the app." "If X, then Y."
- Comma before a coordinating conjunction that joins two independent clauses;
  no comma when the second verb shares the subject.
- Use commas (or a rewrite) to keep clauses short; when a sentence needs many
  commas, split it.

## Colons
https://developers.google.com/style/colons

- Use a colon to introduce a list, a code block, or an explanation that
  completes the setup: "The tool supports three formats: JSON, YAML, and CSV."
- The text before the colon must be able to stand alone (or be a lead-in like
  "the following:"). Don't split a verb from its object with a colon
  ("The formats are: JSON..." is wrong).
- Lowercase after a colon in running text unless a complete sentence or a
  proper noun follows.

## Semicolons
https://developers.google.com/style/semicolons

- Use sparingly. Join two closely related independent clauses, or separate
  list items that themselves contain commas. Often the better fix is two
  sentences or a bulleted list.

## Periods and end punctuation
https://developers.google.com/style/periods

- One space after a period.
- End every complete-sentence list item with a period; no period on fragments
  (see lists rules). No period at the end of headings, captions used as
  titles, or single-fragment table cells.
- Don't end a URL-final sentence in a way that makes the period look like part
  of the URL — prefer link text.
- Question marks: rare in docs; don't use rhetorical questions as headings if
  a statement is clearer (FAQs excepted). Avoid exclamation points.

## Hyphens
https://developers.google.com/style/hyphens

- Hyphenate compound modifiers before a noun ("real-time updates"); don't
  hyphenate after the noun ("updates in real time") or with -ly adverbs
  ("highly available system").
- Prefixes generally close up: pre, re, non, multi, auto, co, meta, anti,
  inter, sub, un → preemptible, nonzero, autoscaling, metafeed. Exceptions
  where the guide keeps the hyphen: multi-cluster, multi-region,
  multi-service, multi-tenancy, non-key, pre-existing, pre-shared key,
  co-worker-type clarity cases, and any case where closing up creates a
  misread (re-create vs recreate) or doubles a vowel awkwardly.
- Use a hyphen for number ranges only in compact contexts; prefer "to"
  ("from 10 to 20") or an en dash in tables.
- Suspended hyphens: "two- and three-node clusters".
- Don't call a hyphen a dash.

## Dashes
https://developers.google.com/style/dashes

- Em dash (—) for a break in thought or an inline expansion — no surrounding
  spaces. Use sparingly; commas or parentheses are often calmer.
- En dash (–) for number ranges in tables and compact text (2010–2020);
  in running text prefer "to" or "through". Don't use an en dash as a minus
  sign in prose; use the word "minus" or code font.

## Parentheses
https://developers.google.com/style/parentheses

- Use for brief asides, abbreviation introductions, and literal references.
  If the parenthetical is a full standalone sentence, punctuate it inside;
  otherwise punctuation goes outside.
- Don't nest parentheses; don't put essential information in them.

## Quotation marks
https://developers.google.com/style/quotation-marks

- Double quotation marks; single only for quotes within quotes.
- American placement: periods and commas inside the closing quote; colons and
  semicolons outside; question marks by sense.
- Exception: when the quoted text is a literal string, filename, or entered
  value, use code font instead of quotes, and keep punctuation outside so the
  reader doesn't type it.
- Titles of short works (articles, episodes) in quotes; full-length works in
  italics — unless the title is link text, then no quotes or italics.
- Don't use quotes for emphasis or so-called scare quotes.

## Slashes
https://developers.google.com/style/slashes

- Don't use "and/or"; rewrite ("A or B", "A, B, or both").
- Don't use slashes to mean alternatives ("on/off" → "on or off") except when
  matching UI text or established notation (A/B testing, I/O, TCP/IP).
- No slashes in dates (1/19/2017 is ambiguous) or in rate units in prose
  (write "per": requests per day, Mbps not Mb/s).
- File paths and URLs keep their slashes in code font; line breaks go after
  the slash.

## Ellipses
https://developers.google.com/style/ellipses

- Avoid in prose. Use only to show omitted text in quoted material or
  truncated code/output, and match UI labels that include them
  ("Save As...": keep the ellipsis when quoting the label but omit it in
  instructions — write "click **Save As**").
