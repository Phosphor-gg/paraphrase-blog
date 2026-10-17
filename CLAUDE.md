# Paraphrase blog

Markdown sources for paraphrase.bot/blog. The website clones this repo at build
time and renders every post, so publishing is adding a file here.

## Writing rules

**No em dashes or en dashes. Ever.** Not `—`, not `–`. Use a comma, a colon,
parentheses, or two sentences. This applies to post bodies, frontmatter,
headings, and commit messages. Check before committing:

```bash
grep -n '—\|–' posts/*.md
```

- British spelling, sentence case for headings.
- Second person ("your episode"), plain language, no hype.
- Contractions are fine. Exclamation marks are not.

## Accuracy

Everything published here is a public claim about a product people pay for, so
it has to survive being quoted back at us.

- **Paraphrase facts come from `research/paraphrase.md`**, which was written
  from the code and the live Stripe setup. If a post needs a Paraphrase fact
  that is not in there, check the code and add it there first, with where it
  came from. Never describe a Paraphrase feature from memory.
- **Competitor claims get checked against their own pages** (pricing page,
  help centre, product pages), read in the session that writes the post. Each
  competitor has a `research/<name>.md` with every fact, the URL it came from
  and the date it was read. A post only states what its research file sources.
- If a page was unreachable, say what the source was and how confident it is,
  or leave the detail out. Do not assert specific limits, prices or feature
  names you could not read.
- Prices change. Every pricing claim says when it was checked.
- Prefer a concrete, checkable statement to a superlative.

## Tone for comparisons

Competitor posts follow a fixed shape: say honestly what the other tool is good
at, explain where its approach differs or runs out, explain what Paraphrase
does differently, and be straight about what Paraphrase does not do. Never
imply a competitor is bad. Most readers already use one and will stop reading
if the post reads as an attack.

Paraphrase is deliberately narrow: it edits your own recording by its
transcript and never generates speech. Most competitors do far more (remote
recording studios, multitrack, voice cloning, captions, music, effects). Say
so plainly; the honest answer for many readers is a competitor, or both.

Open every comparison, alternatives, pricing and listicle post with a bold
**Bottom line:** paragraph that answers the question in the title.

## Format

- `posts/<slug>.md`, filename is the URL slug.
- Frontmatter, quote any value containing a colon:

```yaml
---
title: "Post Title"
date: 2026-10-17
description: "One-line summary shown on the index and in meta tags."
---
```

- `date` is YYYY-MM-DD and drives the index sort, newest first.
- Body starts with `# Title` matching the frontmatter title.
- Standard markdown plus tables.
- Internal links are root relative: `/pricing`, `/docs/ai-cleanup`,
  `/blog/descript-pricing`, `/podcast-editing`.
- Close with a call to action pointing at a free account on
  https://paraphrase.bot or the pricing page.

## Do not

- Edit a published post to change history. Corrections go in a new post.
- Invent testimonials, customer names, user counts or benchmark numbers.
- Claim a feature that is not shipped.
