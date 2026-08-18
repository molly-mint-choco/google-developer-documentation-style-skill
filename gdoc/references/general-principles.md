# General principles

Condensed from the "General principles" category of the Google developer
documentation style guide (CC BY 4.0). Each section lists its source URL.
The sections for voice and tone, global audience, jargon, prescriptive
documentation, and excessive claims are verified against the live pages.

## Voice and tone
https://developers.google.com/style/tone

Target: conversational, friendly, and respectful — a knowledgeable friend who
understands what the developer wants to do. Not slangy, not frivolous, not
pedantic, not pushy. Don't write exactly the way you speak (speech is more
colloquial and verbose), but aim conversational rather than formal. Don't aim
for super-entertaining or super-dry; be human and let personality show, but
remember the reader may be in a hurry — clear, useful information comes first.

Calibration examples (the middle column is the target):

| Too informal | Just right | Too formal |
|---|---|---|
| Dude! This API is totally awesome! | This API lets you collect data about what your users like. | The API documented by this page may enable the acquisition of information pertaining to user preferences. |
| Then—BOOM—just garbage-collect, and you're golden. | To clean up, call the `collectGarbage` method. | Please note that completion of the task requires the following prerequisite: executing an automated memory management function. |

Avoid where possible:
- Buzzwords and technical jargon; being too cutesy; wackiness and goofiness.
- Figurative language, including metaphors and ableist language.
- Placeholder phrases: *please note*, *at this time*.
- Choppy or long-winded sentences; starting every sentence with the same
  phrase (*You can ...*, *To do ...*).
- Current pop-culture references; internet slang and abbreviations
  (*tl;dr*, *ymmv*).
- Exclamation marks (almost always).
- *Let's do X* phrasing.
- *Simply*, *It's easy*, *quickly*, *It's that simple* in procedures.
- Phrasing that denigrates or insults any group of people.

Politeness: don't use *please* in instructions or link introductions.
"To view the document, click **View**." — not "please click **View**".
Reserve *please* for asking a favor, inconveniencing the reader, or flagging a
potential product issue ("If the issue persists, please contact your account
representative.").

Techniques when the tone feels off: ask yourself "What am I trying to say?"
and write that; read the passage aloud and smooth what sounds awkward; add
natural transitions (*Though*, *This way*); when in doubt, prioritize clear
and direct information over perfect tone.

## Write for a global audience
https://developers.google.com/style/translation

Docs are written in US English but translated and read worldwide. Write with
localization (adapting for a country), translation (language conversion), and
internationalization (design that minimizes localization effort) in mind.

Use clear, concise, unambiguous language:
- Use simple words: *start* not *commence*, *so* not *consequently*, *use*
  not *utilize* or *leverage* (unless conveying a special sense, such as
  "utilizes up to 100% of available CPU"). One word over a phrase: *some* or
  *many*, not *a number of*.
- Write shorter sentences. Translations often run longer than the English;
  long sentences impair understanding, break page layouts, and raise
  translation cost.
- Avoid phrasal (compound) verbs when a simpler verb exists: "uses", not
  "makes use of". Accepted exceptions: *set up*, *log in*, *sign in*.
- Limit modifiers: no more than two nouns modifying another noun
  ("a cloud-native DevSecOps pipeline in a hybrid environment", not "a hybrid
  cloud-native DevSecOps pipeline"). Place *only* immediately before the word
  it modifies ("Request only one token", not "Only request one token").
- Active voice, present tense, no complex or uncommon verb forms.
- Use words in their primary sense; don't use one word as noun and verb close
  together; watch ambiguous words (*once*, *while*, *as*, *since*). No
  directional language (*above*, *below*) in procedures.

Use helper and optional words — redundancy that improves comprehension:
- Qualify technical keywords with a noun: "the `example.yaml` file", not bare
  "`example.yaml`".
- Repeat words for clarity: "If the VM has started and **if** you're able to
  connect"; "both IAM **segmentation** and network segmentation".
- Keep *then*, *that*, *of*, and articles: "If the key is not found, **then**
  the default value is returned"; "assumes **that** you have"; "all **of**
  the datasets"; "Start the profiler, **and then** run the app."
- Don't omit relative pronouns: "the rules **that** you previously defined".
- Define abbreviations; abbreviations don't translate well.
- Clarify pronoun antecedents; translators work with small isolated strings,
  so replace an ambiguous *it* with the noun.
- Careful apostrophes: no plurals with 's, no possessives of trademarks, no
  uncommon contractions.

Address users directly: *you*, not *the user* (reserve *the user* for the
people who use the software the reader builds). Provide context; don't assume
prior knowledge. Prefer telling readers what they can do over what they can't.

Be consistent: one term per concept, everywhere, with the same capitalization —
synonyms make translators think you mean different things and raise costs when
translation memory is used. Use standardized phrases for recurring sentences
(link introductions, output introductions, code-sample introductions). Use
subject-verb-object order; keep the subject and verb near the start; put the
conditional clause first; keep list items parallel; keep bold, italics, and
capitalization consistent.

Be inclusive: unambiguous dates and times; no holidays, cultural practices, or
sports unless known worldwide; diverse example names; no colloquialisms,
idioms, or slang (*ballpark figure*, *back burner*); no humor (it rarely
translates); no seasons as time references (August isn't summer everywhere).

Images: use screenshots and figure text sparingly — images don't get
translated. Convey all new information in text.

## Jargon
https://developers.google.com/style/jargon

Jargon is a group's specialized, often figurative terminology (*camel case*,
*swim lane*, *break-glass procedure*, *out-of-the-box*) — and also vague or
overloaded terms (*solution*, *support*, *workload*). It blocks global,
mixed-expertise, and inclusive readership. Some jargon, though, is widely
understood or is what readers search for. Decision path:

1. **Can you write around it?** If SEO doesn't require the term, describe the
   action instead: "When the project is finished, review what worked or
   didn't" rather than "Hold a post-mortem".
2. **Can a more specific term replace it?** Use the word list's replacements:
   *affected area* for *blast radius*, *import* or *load* for *ingest*,
   *ready-made* or *prebuilt* for *off-the-shelf*. Terms marked "Don't use"
   must be replaced or written around.
3. **Used once?** Explain in plain language and put the jargon in parentheses
   — "move the task earlier in the process (also known as *shifting left*)" —
   or link to a trusted definition.
4. **Used throughout?** Define in parentheses on first reference — "a *cold
   standby* (a backup system identical to the primary)" — or link the first
   mention to a trusted definition.
5. **In code or commands?** Use the term only in direct reference to the code
   item, in code font, and make clear what it refers to: "Add a user to the
   allowlist (`whitelist`) by entering ...".

## Prescriptive documentation
https://developers.google.com/style/prescriptive-documentation

Write prescriptive (opinionated) documentation: recommend a way to achieve the
task instead of listing options. When a goal spans multiple approaches or
products, recommend a path. This shapes three things: the document has one
clear purpose and its headings serve it; scenarios and procedures reflect the
most likely use cases; sample commands show the arguments for the most common
case.

Word choice — decide which situation you're in, then pick the verb. Avoid
*should*: it implies "recommended but optional" and leaves the reader unsure.

- **Required action** → *must*, or a plain imperative ("Do the following
  before you continue.").
- **Recommended action** → "We recommend ..." or "COMPANY recommends ...".
  *Should* is tolerable only for generally recognized advice ("You should use
  a strong password").
- **Optional action** → *can* ("You can also use approach B.").
- **Expected outcome** → state it as fact ("The process returns 10 items.").
- **Possible outcome** → *might* or *can* ("The process can take about
  30 minutes.").
- **State of something** → never "The value should be true." Say which you
  mean: "You must set the value to true." / "The server sets the value to
  true." / "If the value is false, follow these steps to change it."

Example fix: "The button should conform to the size guidelines" → "Ensure that
the button conforms to the size guidelines."

## Excessive claims
https://developers.google.com/style/excessive-claims

An excessive claim is a statement that (a) asserts performance or cost the
reader can't verify with available data, (b) asserts security in a way a
single incident would invalidate, or (c) reads as subjective or disparaging,
especially about third-party products. Judge claims against the future, not
just today.

- Avoid superlatives: *best*, *simplest*, *fastest*, *never*, *always*. Use
  *ensure* and *guarantee* only when something truly is ensured or guaranteed.
- Specific performance claims (speed, storage) must cite their source.
- Security: say a feature "helps with security" or "is designed for security"
  — those stay true even after an incident. Not "prevents account takeovers"
  but "is part of an overall strategy that helps prevent account takeovers".
- Competitor comparisons: explain the mechanism and link evidence ("distributes
  computation in memory across a cluster, and therefore can be faster for this
  scenario — see the performance comparison"), never a bare "faster than X".
- Default: factual, objective, verifiable statements that stay true over the
  document's lifespan.

## Accessibility
https://developers.google.com/style/accessibility

- Provide alt text for every meaningful image; make it convey the image's
  purpose, not "image of...".
- Don't convey information by color, size, or position alone ("the red
  button", "the menu on the left", "the section above"). Name the element and
  use "preceding/following" or "earlier/later" for document positions.
- Use meaningful link text (target title or a description), meaningful heading
  hierarchy without skipped levels, and real lists and tables (not ASCII art
  or layout tables).
- Keep sentences short; front-load the important information. Use text
  equivalents for audio and video.
- Refer to people with disability-inclusive phrasing: "person who is blind",
  "screen reader user", "person with a motor disability".

## Inclusive language
https://developers.google.com/style/inclusive-documentation

- Avoid ableist words (crazy, sanity check, cripple, blind to, dumb down),
  gendered words (guys, manpower, he/she as generic), and violent or graphic
  figurative language (nuke, kill in casual senses, STONITH expansions).
- Replace socially charged technical terms: blacklist/whitelist →
  denylist/allowlist; master/slave → primary/replica and similar pairs;
  grandfathered → exempt, legacy; native → built-in.
- Avoid unnecessarily figurative or culturally bound language: idioms, sports
  or military metaphors, US-holiday references (Black Friday → peak scale
  event), "pets versus cattle".
- When a banned term appears in code or a UI you must document, quote it in
  code font, explain it once, and use the preferred term everywhere else.

## Timeless documentation
https://developers.google.com/style/timeless-documentation

- Write as if the doc is read at any time: no "currently", "now", "soon",
  "new", "as of this writing", "does not yet", "eventually", "in the future",
  "latest" (without an anchor).
- Anchor changes to versions or dates: "In versions earlier than 1.17, ...".
- Don't predict roadmaps or promise fixes.

## Future features and pre-announcements
https://developers.google.com/style/future

- Don't pre-announce anything: no hints about unreleased features, launch
  dates, or product direction. Document what exists.

## Third-party content
https://developers.google.com/style/other-sources

- Link to authoritative third-party sources rather than duplicating them.
  Don't copy third-party text into docs without license review; don't rely on
  sources that may disappear or that require sign-in.

## Anthropomorphism (cross-listed)
https://developers.google.com/style/anthropomorphism

- Don't give software human traits: it doesn't "think", "want", "believe",
  "know", or "see". It detects, stores, requires, retrieves, processes.
  Verbs of communication ("the server sends a response") are fine.
