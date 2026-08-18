# Language and grammar

Condensed from the "Language and grammar" category of the Google developer
documentation style guide (CC BY 4.0). Each section lists its source URL.

## Abbreviations
https://developers.google.com/style/abbreviations

- Spell out a term on first use with the abbreviation in parentheses:
  "service level objective (SLO)" — then use the abbreviation. Italicize the
  spelled-out term when introducing it as a definition.
- Don't create abbreviations; use established ones. Don't abbreviate if the
  term appears only once or twice — just spell it out.
- Well-known abbreviations (API, URL, HTML, AI, CPU, REST) need no expansion.
- Don't use Latin abbreviations: e.g. → "for example"; i.e. → "that is";
  etc. → rewrite with "such as" or "including"; vs. → "versus" (except in
  legal case names, "v.").
- Plurals of abbreviations take a plain s: APIs, SDKs, IDs — no apostrophe.
- Pick *a* or *an* by pronunciation of the abbreviation: a SQL, an SLA,
  an HTML file, a URL, a FHIR, an SAP system.
- Don't abbreviate in headings when the term is unfamiliar; the heading may
  be the reader's entry point.

## Active voice
https://developers.google.com/style/voice

- Prefer active voice: "The compiler reports the error", not "The error is
  reported". Active voice names the actor, which matters in docs — the reader
  must know whether they act or the system does.
- Passive voice is acceptable when the actor is unknown or irrelevant, or to
  avoid blaming the reader ("the file was deleted").
- Watch for hidden passives: "the file needs to be saved" → "save the file".

## Articles (a, an, the)
https://developers.google.com/style/articles

- Include articles; dropping them ("Click button to save file") reads like a
  telegraph and translates poorly.
- a/an by sound, not spelling: a user, an hour, a URL, an SDK.
- No "the" before most product names; "the" before tool and API names
  (the Transcoder API, the `gcloud` CLI). See references/html-naming.md.

## Capitalization
https://developers.google.com/style/capitalization

- Sentence case everywhere: headings, titles, table headers, list items,
  navigation. Capitalize only the first word, proper nouns, and the first
  word after a colon in a heading.
- Don't use capitalization for emphasis or to invent proper nouns for
  ordinary features ("the export feature", not "the Export Feature").
- Match official capitalization of products, languages, and brands
  (macOS, iOS, Kubernetes Pods/Jobs when following upstream docs).
- Hyphenated words in sentence case: capitalize only the first element unless
  the second is a proper noun ("Built-in functions").
- After a colon in running text, lowercase unless what follows is a complete
  sentence or a proper noun.

## Contractions
https://developers.google.com/style/contractions

- Use common contractions (it's, don't, you're, isn't); they make tone
  friendly. "isn't" and "don't" are clearer than "is not" for negation
  emphasis in some cases, but negative contractions also help readers not
  miss the "not".
- Avoid noun+verb contractions ("the browser's fast") — ambiguous with
  possessives. Avoid double contractions (mustn't've) and *let's*.

## Pluralization
https://developers.google.com/style/pluralization

- Plural of a code item or filename: add "s" outside code font is wrong —
  instead pluralize the concept: "`Widget` objects", not "`Widget`s".
  If unavoidable, write "Widgets" in plain text.
- Don't use "(s)" — write "one or more files", or just the plural.
- Letters-as-letters and abbreviations: APIs, the 2020s, x-values.

## Possessives
https://developers.google.com/style/possessives

- Singular nouns take 's even when ending in s ("the OS's kernel" — but
  prefer rewriting: "the kernel of the OS").
- Don't form possessives of product, company, or feature names ("the Google
  Cloud console menu", not "Google Cloud console's menu") and never of
  trademarks. Rewrite with "of" or use the name attributively.
- Don't form possessives of code items in code font.
- its = possessive; it's = it is.

## Prepositions
https://developers.google.com/style/prepositions

- Ending a sentence with a preposition is fine when natural.
- Standard pairings: in a field/dialog/window, on a page/tab/toolbar, in the
  console, on the command line, in a directory, click X (no "on"),
  type in a box, appears in a list, sign in to (never "sign into"),
  listen on a port, authenticate against.

## Present tense
https://developers.google.com/style/tense

- Default to present tense: "The command creates a file", not "will create".
- Use future tense only for genuine future events from the reader's timeline.
  Avoid "would", "could", "used to".
- Timeless truth over sequence-of-events narration.

## Pronouns
https://developers.google.com/style/pronouns

- Singular "they/them/their" as the generic pronoun; never generic "he",
  "she", "he/she", "(s)he".
- Ensure a pronoun's antecedent is unmistakable; repeat the noun when "it",
  "this", or "that" could point at two things. Prefer "this setting" over a
  bare "this".
- Don't use "one" as a pronoun.

## Second person
https://developers.google.com/style/person

- Address the reader as "you". Don't use "we" for actions the reader takes
  ("we then create a bucket" → "create a bucket"). "We" is acceptable only as
  the documentation's authors ("we recommend").
- Imperative mood for instructions.
- Establish who "you" is if the doc serves multiple roles (admin vs developer).

## Sentence structure
https://developers.google.com/style/sentence-structure

- Put conditions, goals, and locations before the action:
  "To create a cluster, run:", "If the light is red, stop",
  "In the **Name** box, enter a value". The reader can then skip steps that
  don't apply.
- One main idea per sentence; break up long sentences.

## Verbs in reference documents
https://developers.google.com/style/reference-verbs

- API descriptions: start method/function descriptions with a present-tense,
  third-person verb: "Creates a new user.", "Returns the list of jobs."
- Describe what it does, not what it "will do" or what "you can use it to do".
- For fields and parameters, use noun phrases or "The ID of the ...".

## Spelling
https://developers.google.com/style/spelling

- American English, Merriam-Webster first-listed form: canceled, traveling,
  color, license (noun and verb), gray, adviser.
- Exception: match official names and code exactly.
