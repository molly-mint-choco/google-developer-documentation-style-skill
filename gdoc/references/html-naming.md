# HTML, Markdown, and naming

Condensed from the "HTML and CSS", "Names and naming", and "Product names"
pages of the Google developer documentation style guide (CC BY 4.0).

## Markdown versus HTML
https://developers.google.com/style/markdown

- Use Markdown by default; drop to HTML only for what Markdown can't do
  (definition lists, complex tables, `<var>`, semantic tags).
- Be consistent within a document; don't mix syntaxes for the same construct.
- Markdown conventions: `**bold**` (not `__`), `_italic_` (not `*`),
  backticks for code, `-` for bullets, ordered lists numbered `1.`.

## HTML and semantic tagging
https://developers.google.com/style/semantic-tagging

- Use elements for meaning, not looks: `<em>` for emphasis, `<strong>` for
  strong importance, `<code>` for code, `<var>` for placeholders, `<kbd>` for
  keypresses, real `<table>`, `<ol>`, `<ul>`, `<dl>` structures.
- Don't fake styling with `<b>`, `<i>`, inline CSS, or manual monospace
  fonts; don't override global font type, size, or color.
- Sequential heading levels; alt attributes on images.

## HTML formatting
https://developers.google.com/style/html-formatting

- Lowercase element and attribute names, quoted attribute values, two-space
  indents, no trailing whitespace. Close elements that require it; keep void
  elements bare (`<br>`, not `<br/>`).

## Example domains and names
https://developers.google.com/style/examples

- Domains: use `example.com`, `example.org`, `example.net` and subdomains
  (RFC 2606). Never a real company's domain.
- Email addresses: use example.com addresses. People: use clearly diverse,
  fictional names, or role names (Alex, Dana; "the administrator").
- IP addresses: use the documentation ranges 192.0.2.0/24, 198.51.100.0/24,
  203.0.113.0/24, and 2001:db8::/32 for IPv6. Phone numbers: +1-XXX-555-01XX.
- Avoid foo/bar/baz; pick meaningful sample names (`my-sample-bucket` as a
  literal example value).
- Don't use real personal data, credentials, or keys — even expired ones.

## Filenames
https://developers.google.com/style/filenames

- Name new files and directories with lowercase letters and hyphens between
  words: `getting-started.md`, `data-retention-policy.html`. Avoid
  underscores, spaces, and camelCase unless the platform requires them.
- Keep names short, descriptive, and stable (they become URLs).
- In prose, filenames go in code font.

## Trademarks
https://developers.google.com/style/trademarks

- Use trademarked names as adjectives-with-noun on first use where required
  by the owner's guidelines, spell them exactly, and never inflect them: no
  plurals, possessives, verbs, or abbreviations of trademarks.
- Don't incorporate third-party trademarks into your product's name or
  feature names. Follow each owner's published trademark guidelines
  (Google's own list: https://www.google.com/permissions/trademark/trademark-list/).
- Trademark symbols (™, ®) are generally not required in documentation body
  text; follow your legal team's rules.

## Product names
https://developers.google.com/style/product-names

- Google product names are title case; follow official capitalization of any
  brand, product, or open source term (Kubernetes Pods and Jobs when the
  upstream docs capitalize them; macOS stays lowercase even at risk of
  sentence-start — rewrite the sentence instead).
- Feature names are lowercase unless officially capitalized or matching a UI
  label.
- Don't abbreviate product names (no GCP); use the full trademarked name, or
  shift to a generic term after first mention ("a service mesh").
- Articles: no "the" before product names ("using Cloud Datastore"); "the"
  before tool and API names ("the Transcoder API", "the `gcloud` CLI",
  "the Google Cloud console").
- Indefinite article by sound of the actual first word ("an Anthos Service
  Mesh environment", "a Service Mesh environment").
- It's OK to call products "services" unless ambiguous.
- Never use product or feature names as verbs ("search with Google", not
  "google it").
- Possessives: don't form them from product or company names; rewrite with
  "of" or use the name attributively.
