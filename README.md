# Paraphrase blog

Markdown sources for [paraphrase.bot/blog](https://paraphrase.bot/blog).

The website builds the blog from this repo: a pre-build step clones it,
renders every post to HTML and generates the date-sorted index, so publishing
is adding a markdown file to `posts/` and rebuilding the website.

`research/` holds the sourced facts every post is written from: one file per
competitor (each fact with the page it came from and when it was read) and
`paraphrase.md` for Paraphrase itself. See `CLAUDE.md` for the rules.
