# Formatting and organization

Condensed from the "Formatting and organization" category of the Google
developer documentation style guide (CC BY 4.0). Each section lists its
source URL.

## Headings and titles
https://developers.google.com/style/headings

- Sentence case. No terminal period. No ampersands.
- Use a task-based gerund or imperative for procedures ("Creating a cluster"
  or "Create a cluster" — pick one style per doc set; current Google practice
  favors bare imperative/infinitive).
- Keep heading levels sequential (h2 then h3; don't skip). Exactly one h1.
- Make headings unique within a page, descriptive, and parallel in structure.
- Don't stack a heading directly on another heading without intervening text
  where the child heading needs framing; a short intro sentence helps.
- Don't put code font as the entire heading if avoidable; if a code item must
  appear, code font is OK inside the heading.
- Avoid questions as headings except in FAQs.

## Paragraphs
https://developers.google.com/style/paragraph-structure

- Lead with the point (BLUF). One topic per paragraph; three-to-five
  sentences is a good ceiling.
- Put critical warnings before the step they affect, not after.

## Lists
https://developers.google.com/style/lists

- Numbered list = sequence of steps; bulleted list = unordered set;
  description list = pairs of related data (term and definition).
- Every list needs an introductory sentence or fragment ending in a colon
  (complete sentence preferred).
- Items must be grammatically parallel. Capitalize the first word of each
  item.
- Punctuation: if any item is a complete sentence, end all items with
  periods; single words or short fragments take no period.
- Run-in headings in lists: bold the leading term, follow with a colon or
  period, then the explanation.
- Don't use a list when a sentence with three short items reads fine; don't
  exceed one level of nesting when possible.
- Steps that are optional start with "Optional:".

## Procedures
https://developers.google.com/style/procedures

- Number the steps; one action per step. A short result statement ("The
  **Settings** page opens.") may share the step.
- Write steps in the imperative and in the order the reader performs them,
  condition first: "In the **Name** field, enter a name."
- Combine tiny actions with angle-bracket menu paths sparingly: prefer
  "click **File > New > Document**" style (bold each label, spaces around >).
- State the goal before the steps ("To export the data, follow these steps:").
- A single-step procedure is a bulleted single item, not "1.".
- Tell readers about prerequisites ("Before you begin") before the first step.
- Don't bury a second required action inside a step's explanation.
- For long procedures, group steps under sub-headings or split into stages.

## Notes and other notices
https://developers.google.com/style/notices

- Types: **Note** (useful aside), **Caution** (potential problem — proceed
  carefully), **Warning** (danger of data loss, security exposure, money),
  plus product-stage notices (Preview, Deprecated).
- Place the notice before the content it affects. Keep notices rare — a page
  of callouts means the structure is wrong. Don't stack notices back-to-back.
- Format: bold run-in label, then the text.

## Numbers
https://developers.google.com/style/numbers

- Spell out zero through nine; numerals for 10 and up — with exceptions:
  always numerals for versions, page/chapter/step numbers, units of
  measurement, percentages, dimensions, and numbers the reader compares or
  computes.
- Don't start a sentence with a numeral; rewrite or spell it out.
- Use commas in numbers of four or more digits (1,024) except years, ports,
  addresses, and code.
- Ranges: "10 to 20", or an en dash in tables. "More than" not "over" for
  quantities; "approximately" not "~" in prose.
- Fractions as decimals in technical text (0.5); "half" in casual text.
- Ordinals spelled out (first, second) — don't use 1st, 2nd.

## Dates and times
https://developers.google.com/style/dates-times

- Dates: "January 19, 2017"; abbreviate months only when space demands
  (Jan 19, 2017). Never all-numeric dates.
- For date-only machine formats use ISO 8601 (2017-01-19) and say so.
- Times: 9:00 AM (space, caps, no periods); include time zone when it
  matters, preferably as UTC offset.
- Durations: spell the unit (30 seconds, 5 minutes); use HH:MM:SS only in
  tables or UI matching.
- Don't use seasons as time anchors.

## Tables
https://developers.google.com/style/tables

- Use tables for parallel structured data, not for layout, not for a single
  row, and not when a list is clearer.
- Introduce every table with a sentence ("The following table describes ...").
  Refer to it by "the following table" or a numbered caption, never "the
  table below".
- Column headers: sentence case, bold by default markup, no terminal
  punctuation. Keep cell text parallel; fragments don't take periods.
- Don't leave cells empty — use "None" or an em dash with header context.
- Sort rows in a sensible, stated order.

## Format examples
https://developers.google.com/style/format-examples

- Introduce examples with "for example," or "such as", or a lead-in sentence
  ending in a colon for block examples.
- Keep examples realistic, minimal, and runnable where applicable; show
  output when it helps.
- "For example" starts a new sentence for long examples; parentheses or
  dashes set off short inline ones.

## Figures and other images
https://developers.google.com/style/images

- Use images to supplement text, never to replace it; the doc must make sense
  with images stripped.
- Every image needs alt text (unless purely decorative); complex figures need
  a text description nearby or a long description link.
- Use high-resolution or vector (SVG) images. Crop screenshots to the
  relevant region; don't include personal data; prefer showing UI states the
  reader can reach.
- Introduce figures in text ("The following diagram shows ..."). Captions are
  sentence case: "Figure 1. The request lifecycle."
- Don't embed critical text only inside an image.

## Italics with terms
https://developers.google.com/style/italics-terms

- Italicize a term when defining it or discussing the word itself:
  "A *shard* is ...". Use italics for that first mention only; plain
  thereafter.
- Don't use italics for emphasis freely; usually the sentence can carry it.

## Footnotes
https://developers.google.com/style/footnotes

- Avoid footnotes. Work information into the text, a notice, or a link.
  In tables where a footnote is unavoidable, use superscript numbers and
  place notes directly under the table.

## Mathematical notation
https://developers.google.com/style/mathematical-notation

- Italicize variables (*x*, *n*); roman for operators, functions, and units.
- Use real symbols (×, ≤) or MathJax for display math, not code-y
  approximations (<=) in prose. Code font when the math is literally code.
- Define every variable when introduced.

## Phone numbers
https://developers.google.com/style/phone-numbers

- Write in international format with country code: +1-650-555-0100.
  Use reserved fictional numbers (555-01xx range) in examples.

## Units of measurement
https://developers.google.com/style/units-of-measure

- Space between number and unit (64 GB); no space with % and ° in technical
  usage per SI conventions the guide follows (360°, but "64 GB", "10 Mbps").
- Binary vs decimal: use the unit the product uses; don't mix GB and GiB
  meanings silently.
- Rates with "per" in prose (requests per second); slash only where space is
  tight. MBps = megabytes per second, Mbps = megabits — never MB/s or Mb/s.
- Don't pluralize unit symbols (5 kg, not 5 kgs); spell out the unit on first
  use if it's uncommon.
