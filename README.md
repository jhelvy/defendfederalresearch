# Defend Federal Research

A public guide to help researchers and the public submit **public comments** on the
U.S. Office of Management and Budget's proposed rule, *Regulation for Federal Financial
Assistance* — a government-wide overhaul of the rules governing federal grants.

🌐 **Live site: <https://defendfederalresearch.org>**

> **Comment deadline: July 13, 2026** · Docket **OMB-2026-0034** · submit at
> [regulations.gov](https://www.regulations.gov/docket/OMB-2026-0034)

This is an independent, volunteer-built project. It is **not** affiliated with OMB or any
federal agency, and nothing here is legal advice.

## What's in the guide

- **The Rule, Section by Section** — plain-language analysis of every meaningful change,
  with the rule's own quoted text, an impact note, and a suggested talking point per section.
- **Claims vs. Reality** — rebuttals to OMB's stated justifications (transparency, reduced
  burden, open science, lawful oversight).
- **How to Comment** — step-by-step instructions, including the required `[section]` bracket
  format and what makes a comment count.
- **Draft with AI** — a copy-paste prompt that turns a researcher's situation into a
  personalized, section-specific draft comment (with guardrails to personalize and verify).
- **Contact Congress** — find your representatives and reuse your comment as a message to them.
- **FAQ** and **Resources**.

## How it's built

- [Quarto](https://quarto.org) website (Markdown → static HTML), themed with `styles.scss`.
- Client-side full-text search, and `llms-txt: true` generates an `llms.txt` index plus a
  `.llms.md` copy of every page so AI assistants can read the analysis directly.
- Hosted on **GitHub Pages** at a custom domain (`CNAME`), deployed automatically from `main`
  to the `gh-pages` branch via GitHub Actions (`.github/workflows/main.yml`).

## Run it locally

Requires [Quarto](https://quarto.org/docs/get-started/) (≥ 1.7 for `llms.txt` generation).

```bash
quarto preview   # live-reloading local server
quarto render    # build the full site into _site/
```

No R packages are required to build the site (it contains no executable code cells).

## Project structure

```
index.qmd            Home
the-rule.qmd         Section-by-section guide
claims-vs-reality.qmd
how-to-comment.qmd
draft-with-ai.qmd
contact-congress.qmd
faq.qmd  resources.qmd  about.qmd
_countdown.qmd       Deadline-countdown partial (included by the home page)
_quarto.yml          Site config (navbar, theme, llms.txt, custom domain resource)
_variables.yml       Central values (site URL, docket, deadline) used via {{< var >}}
styles.scss          Theme
2026-10817.md/.pdf   Full text of the proposed rule (source for the analysis)
guides/              Reference comment guides from other organizations
```

When the site moves to a new URL, update `site.url` in `_variables.yml` **and** `site-url`
in `_quarto.yml` (Quarto config cannot read the variables file).

## Contributing

Corrections and additions are welcome — accuracy matters here. Especially useful:

- Fixes where anything misstates the rule (cite the section so it can be verified against the
  [source](https://www.regulations.gov/docket/OMB-2026-0034)).
- Discipline-specific talking points and examples.
- A share kit (social posts, graphics) to help spread the word.

Please open an issue or pull request.

## License

Content is licensed **CC BY-SA 4.0**. You are free to share and adapt it with attribution
under the same license.
