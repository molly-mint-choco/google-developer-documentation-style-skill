# Word list (curated)

Source: https://developers.google.com/style/word-list (CC BY 4.0).
This file condenses the entries writers hit most often. For any term not
listed here, fetch the source page and search for the term; if it isn't there,
use Merriam-Webster's first-listed spelling.

Severity labels:
- **Don't use** — never use the term.
- **Avoid** — use only if it's clearly the best choice; prefer the alternative.
- Exception: if a UI label, command, or code item uses a banned term, quote it
  exactly in code font or bold, make clear what you refer to, and use the
  preferred term elsewhere.

## Banned or replaced terms

| Don't use | Use instead |
|---|---|
| abort | stop, exit, cancel, end |
| agnostic | platform-independent |
| aka | also known as, or |
| allows you to, enables you to | lets you |
| and/or | rewrite; or "A or B or both" |
| blacklist / whitelist / graylist | denylist, blocklist / allowlist / provisional list (nouns only; rewrite verbs) |
| black hat / gray hat / white hat | illegal, unethical, ethical, in violation of rules |
| blast radius | affected area, spatial impact |
| check / uncheck / deselect (a checkbox) | select / clear |
| click here, this link | descriptive link text |
| click on | click |
| cons / pros | disadvantages / advantages |
| comprise | consist of, contain, include |
| crazy, insane | complicated, unexpected (objects only) |
| cripple, gimp, lame | precise non-figurative wording (slowed, reduced) |
| desired | that you want |
| disable(d) for broken things | not responding, unavailable, inactive, turned off |
| drag and drop (verb) | drag ("drag-and-drop" OK as adjective) |
| dummy variable | placeholder |
| e.g. / i.e. | for example, such as / that is |
| email (verb) | send email |
| etc., and so on | "such as ..." or "including ..." |
| female/male adapter | socket / plug |
| grandfathered | legacy, exempt |
| grayed-out | unavailable |
| guys | everyone, folks |
| hamburger menu, kebab menu | the icon's aria-label, e.g. **Menu**, **More** |
| hang / hung | stop responding, not responding |
| he, she (generic) | they |
| hit | click, press, type |
| hover | hold the pointer over; or point to |
| impact (verb) | affect |
| in order to | to (unless needed for clarity) |
| kill | stop, exit, cancel, end |
| k8s | Kubernetes |
| leverage | use, build on |
| log in / log out (verbs) | sign in / sign out |
| man-in-the-middle | on-path attacker, person-in-the-middle (PITM) |
| manned, manpower, man-hours | staffed/crewed, staff/workforce, person-hours |
| master / slave | primary/replica, controller/worker, leader/follower, main |
| MIME type | media type |
| mobile (noun), cell phone, smartphone | mobile phone; mobile device |
| native (for features) | built-in |
| omnibox | address bar |
| please (in instructions) | omit |
| pop-up | dialog (window); menu |
| regex | regular expression |
| repo | repository |
| sane, sanity check | valid, sensible; quick check, confidence check |
| should | must (required), can (optional), might (possible) |
| simple, simply, easy, easily, quick, just | omit; the reader decides what's easy |
| slave | worker, replica, secondary |
| smartphone | mobile phone, phone |
| spin up | create, start |
| ssh (verb) | connect using SSH; use the `ssh` command |
| terminate ≠ delete; deprecate ≠ remove | use the precise action word |
| uncheck | clear |
| utilize | use |
| wish, desire | want, need |
| zippy, expando | expander arrow, expandable section |

## Spelling of compounds (correct forms)

One word, no hyphen: autoscaling, autopopulate, backend, frontend, codebase,
dataset, datastore, ecommerce, endpoint, filename, healthcare, hostname,
hardcoded, intercluster, inline, lifecycle, livestream, metadata, microservices,
namespace, prebuilt, preemptible, prerecorded, presubmit, runbook, runtime
(environment), screenshot, username, workflow.

Two words: data center, data source, data type, file system, key ring,
name server, plain text (except cryptography: plaintext), home screen,
lock screen, status bar, web page, run time (moment during execution).

Hyphenated: big-endian, little-endian, blue-green, double-click, right-click,
drop-down (adjective; prefer plain "list"/"menu"), error-prone, key-value pair,
multi-cluster, multi-region, multi-service, multi-tenancy, non-key,
on-premises (never "on-premise"), pre-existing, pre-shared key, read-only,
single sign-on.

Noun vs verb pairs: login / log in, setup / set up, startup / start up,
backup / back up, failover / fail over, sign-in / sign in, checkout / check out,
rollback / roll back, workaround / work around.

Casing: internet (lower), web (lower), boolean (lower unless language keyword
or Boolean logic), base64, curl (not cURL), IPsec, HTTPS, ID (not Id), I/O,
IoT, OAuth 2.0, NoSQL, DNSKEY, Wi-Fi, macOS, PoP, MBps (bytes) vs Mbps (bits —
never MB/s), gRPC-style official casing always wins.

## Usage distinctions

- **can / might / must / may**: can = ability or permission; might =
  possibility; must = requirement; may = reserve for legal or policy meaning.
- **because vs since/as**: use *because* for causation; *since* and *as* are
  time words.
- **after vs once**: use *after*.
- **whether vs if**: use *whether* for alternatives ("whether the flag is
  set"); *if* for conditions. Write "whether or not" only when both outcomes
  need equal weight; include "then" in if–then sentences.
- **between vs among**: between = distinct items (two or more); among = group
  membership.
- **each vs all**: each = individually; write "a list of all the items", not
  "a list of each item".
- **select vs click vs tap vs press**: select for choosing options and marking
  checkboxes; click for mouse targets on desktop; tap for touchscreens and
  Android; press for physical keys and key combos (`Control+S`, note the plus,
  and mention `Command` for macOS).
- **enter vs type**: enter = put text in a field (may include pasting);
  type = literally type. Don't write "copy and paste" as an instruction —
  say what to enter.
- **fill in** (a field) vs **fill out** (a form).
- **earlier / later** for version ranges, not lower/higher/above/below
  (Android docs invert this: use lower/higher).
- **later / following / earlier / preceding** for positions in a document,
  never above/below.
- **authenticate** (a user proves identity) vs **authorize** (a request acts
  on the user's behalf). Not authN/authZ.
- **deprecate** = discourage use, announce end of support. Not a synonym for
  removed or deleted.
- **data** is singular and a mass noun: "the data is", "less data".
- **appendixes, indexes, matrixes, schemas** — English plurals, unless
  mathematical context demands indices/matrices.
- **emoji** is its own plural.
- **directory** in command-line contexts; **folder** in GUI contexts.
- **dialog** for the UI element; **dialogue** for conversation between people.
- **app** for consumer software; **application** in formal phrases and
  enterprise contexts.
- **for example**, followed by a comma. *Like* and *such as* are both fine
  for examples; don't write "for instance" (collides with compute instances).
- **per**: rates only ("requests per day"); not "per the style guide" or
  "per Pod" (write "according to", "for each").
- **display** is transitive: "the page appears" or "the page is displayed",
  never "the page displays" without an object.
- **populate** for processes; **fill in** for people.
- **exploit** only in the security sense, never meaning "use".
- **ingest** only for load-plus-processing; else import, load, copy.
- **execute** → prefer *run*.
- **extract** archives; don't unzip/untar in prose.
- **listen on** a port, not "listen to".
- **timeless words to cut**: currently, now, soon, new, latest (without a
  version anchor), eventually, in the future, as of this writing, does not yet.

## First-use expansion rules

Spell out on first use, abbreviation after: infrastructure as a service (IaaS),
platform as a service (PaaS), software as a service (SaaS), fintech, ad tech,
Identity and Access Management (IAM), DNSSEC, IDN, IKE, LOA-CFA, SLA, SLI, SLO,
long-running operation (LRO), managed instance group (MIG).

No expansion needed: API, CPU, AI, DevOps, REST (never expand REST), SSH, URL,
HTML, IPsec, OS.

Article choice goes by sound: *a SQL* ("sequel"), *an SAP* ("ess-ay-pee"),
*a FHIR* ("fire"), *an HTML page*, *a URL*.

## Google-specific names

- *Google Cloud*, never GCP or "Cloud" alone. *Google Cloud console* (then
  "the console"); always "the" before console names. *Google Cloud CLI* on
  first mention, then `gcloud` CLI.
- *Google Account* (capital A). *Google Play services* (lowercase s).
  *Google I/O*. *2-Step Verification* (Google's product; generic is lowercase).
- Don't use *Cloud SDK* variants, *API Console*, *Developers Console*,
  *dashboard*, or *portal* for the Google Cloud console.
- alpha, beta lowercase except in product names ("PRODUCT Beta").

## Note on coverage

The live word list continues past this file's coverage (terms from S–Z such as
tap, touch & hold, turn on, US, via, and web-related compounds appear on the
source page). When you review a term this file doesn't settle, fetch
https://developers.google.com/style/word-list and search the page before ruling.
