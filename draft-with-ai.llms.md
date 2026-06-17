# Draft a Comment with AI

An AI assistant (Claude, ChatGPT, or similar) can turn *your* situation into a solid first draft in a couple of minutes. Used well, it lowers the barrier to writing a **specific, personal** comment — which is exactly the kind that counts.

> **WARNING:**
>
> - **The draft is a starting point, not a finished comment.** Edit it so it sounds like you.
> - **Verify every fact, number, and claim** before you submit — AI can invent things.
> - **Never submit text you haven’t read.** Your name goes on the public record.
> - **Don’t share the prompt as a “just submit this” form letter.** Identical comments get collapsed into one. The whole point is that yours is genuinely yours.

## The prompt

Copy this into your AI assistant, fill in the **ABOUT ME** section, and edit the result.

``` markdown
You are helping me write a public comment on a proposed U.S. federal regulation:
the OMB "Regulation for Federal Financial Assistance" (Docket OMB-2026-0034), a
government-wide overhaul of the rules for federal grants and cooperative agreements.

CONTEXT — read this first if you are able to browse the web:
A plain-language, section-by-section analysis of the proposed rule, with the rule's
own text, is published here:
  https://REPLACE-WITH-SITE-DOMAIN/llms.txt
To focus on a specific section, read its page, for example:
  https://REPLACE-WITH-SITE-DOMAIN/sections/section-200-205.llms.md
If you cannot browse the web, tell me and I will paste the relevant section text.

ABOUT ME — replace everything in brackets:
- Field / discipline: [e.g., structural biology]
- Role and institution type: [e.g., tenure-track PI at an R1 university]
- Funding I rely on: [e.g., NIH R01, NSF CAREER]
- What I actually do day to day: [1–2 sentences]
- The section(s) that worry me most: [e.g., 200.205, 200.340, 200.220]
- Concrete ways this rule would damage my work or field: [your real examples]

TASK:
Write a public comment of about 300–500 words that:
1. Begins with the section number in brackets, e.g. "[200.205]".
2. Is written in my own voice, grounded in the specifics I gave above.
3. Makes 2–3 concrete, factual points about real-world harm — not slogans or partisanship.
4. Stays professional and respectful in tone.
5. Reads like a specific, credible expert wrote it — not a form letter.
Then give me a short checklist of any facts, numbers, or claims I should verify
before I submit.
```

## How to use it

**If your assistant can browse the web** (e.g., Claude with web access, or ChatGPT with browsing): it will read our analysis at `llms.txt` and the specific section pages, so its draft reflects what the rule actually says.

**If it can’t browse:** open the [section guide](sections/index.llms.md), copy the text of the section(s) you care about into the chat when it asks, and it will work from that.

> **TIP:**
>
> This site automatically publishes a machine-readable copy of every page (an `llms.txt` index plus a `.llms.md` version of each page). That lets an AI assistant read our actual analysis and the rule’s own wording, instead of guessing — so the draft it gives you is grounded, not hallucinated.

## Before you submit

- Read the whole draft and rewrite anything that doesn’t sound like you.
- Check it opens with the right `[section]` bracket.
- Verify the facts on the model’s checklist.
- Submit at [regulations.gov, Docket OMB-2026-0034](https://www.regulations.gov/docket/OMB-2026-0034). See [How to Comment](how-to-comment.llms.md) for the walkthrough.
