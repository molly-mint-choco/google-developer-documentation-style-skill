# Computer interfaces

Condensed from the "Computer interfaces" category of the Google developer
documentation style guide (CC BY 4.0). Each section lists its source URL.

## Code in text
https://developers.google.com/style/code-in-text

Put in code font (`<code>` or backticks): attribute names and values, class,
method, and function names; command names and command-line utility names
(`gcloud`, `curl`, `ssh` as the utility); data types; defined constants and
enums; environment variables; element names; filenames, extensions, and paths;
folders and directories; HTTP verbs, status codes, and content-type values;
IP addresses; ports; query parameters; strings the user enters or the system
returns; URLs used as literal values; placeholders.

Not in code font: product, service, and API names (the Cloud Storage API);
concepts named after code (a bucket, a pod as a concept when following prose
usage); keyboard keys use code font per key (`Enter`, `Control+C`).

- Don't inflect code items: no possessives, no added plurals inside the code
  font. Rewrite around them ("`Widget` objects").
- When a sentence starts with a lowercase code item, rewrite the sentence
  rather than capitalizing the code.

## Code samples
https://developers.google.com/style/code-samples

- Introduce each sample with a sentence that says what it does, ending in a
  colon if the sample immediately follows.
- Samples must be correct, minimal, self-contained where practical, and follow
  the language's own style guide. Prefer runnable over pseudo.
- Wrap lines at about 80 characters; break long commands with the shell's
  continuation character (`\`) at logical points.
- Mark placeholders clearly (see below) and explain each one after the block:
  "Replace the following: PROJECT_ID: the ID of your project."
- Show expected output separately from input when confusion is possible; you
  can label the output block or introduce it ("The output is similar to the
  following:").
- Don't include prompts (`$`) unless you need to distinguish input from
  output; be consistent.
- Don't put optional and required arguments together without marking them
  (see command-line syntax).
- Provide context: state where the code runs (Cloud Shell, local terminal)
  and prerequisites.

## Command-line syntax
https://developers.google.com/style/code-syntax

- Document syntax with these conventions: required arguments in plain code;
  optional parts in square brackets `[--flag=VALUE]`; mutually exclusive
  choices grouped and pipe-separated; repeatable items with ellipsis
  `FILE ...`; placeholders in caps.
- Flags: give the full form; list default values; put the flag before
  positional args in examples if the tool allows.
- Use `Control+C`-style key notation to stop processes; naming Linux signals
  (SIGKILL) is the exception where "kill" terminology is acceptable, quoting
  the technical term.
- Show one command per block when steps are sequential; don't chain with `&&`
  in teaching material unless the chaining is the point.

## Placeholder formatting
https://developers.google.com/style/placeholders

- Placeholder text: UPPERCASE_WITH_UNDERSCORES, in code font; in HTML also
  wrap in `<var>`.
- Choose descriptive names: `BUCKET_NAME`, `REGION` — not `XXX`, `foo`, or
  `my-thing` as the placeholder itself (example values like `my-bucket` are
  fine as sample literals, but then they're examples, not placeholders).
- Immediately after the code block, list each placeholder and what to replace
  it with ("Replace the following:").
- Don't reuse one placeholder for two meanings on the same page.

## UI elements and interaction
https://developers.google.com/style/ui-elements

- Bold the names of UI elements the reader interacts with: buttons, menu
  items, dialog titles, field labels, checkboxes, tabs. Match the UI's
  capitalization exactly, even when it breaks style rules.
- Don't bold the generic noun: "click **Save**", "the **Name** field" —
  "field" stays plain.
- Menu paths: "select **File > New > Project**" (bold labels, > separator).
- Element vocabulary: button (click/tap), checkbox (select/clear), toggle
  (click, or "turn on"), list and menu (select an item; drop the word
  "drop-down" unless needed), dialog (in a dialog, click ...), field/box
  (enter a value in), tab (click the ... tab), window/pane/panel, navigation
  menu (not left nav), expander arrow.
- Verbs: click (mouse), tap (touch/Android), press (physical keys), enter
  (put text), select/clear (checkboxes and options), drag (not drag and
  drop), hold the pointer over (when the UI must react; otherwise point to),
  go to (a page).
- Don't describe the UI's look ("the little gear icon at the top right");
  name the element and its aria-label: "click settings **Settings**".
- Write UI text itself (if you're producing it) in sentence case, short,
  verb-first for buttons.

## API reference code comments
https://developers.google.com/style/api-reference-comments

- Method/function summaries: begin with a present-tense third-person verb:
  "Deletes the specified instance." First sentence stands alone as the
  summary.
- Parameters: define each; state type, whether optional, default value, and
  constraints. Booleans: describe what true and false each mean.
- Return values: "Returns X if ..., otherwise Y." Document errors/exceptions
  and when they're raised.
- Classes: start with what an instance represents. Constants and fields:
  noun phrases.
- Keep comments in the code style of the language (Javadoc, docstrings) and
  follow the same word-list and tense rules as prose.
