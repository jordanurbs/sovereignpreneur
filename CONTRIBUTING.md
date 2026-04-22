# Contributing

Thank you for reading the declaration closely enough to want to edit it. Here's how to do that well.

## Editorial stance

**The four axioms are fixed.** Deflation, the reference frame, production, agency. PRs that propose replacing or adding axioms will be closed. If you think an axiom is wrong, open an Issue and argue it — don't ship a fork.

**The language around the axioms is meant to sharpen over time.** That's where contributions live: clearer phrasings, better examples, stronger sources, fixed typos, broken-link patches, new figures.

**Every revision should make the document more precise, not more comprehensive.** If an edit adds length without adding precision, it won't land.

## What belongs in a PR

- Typos, grammar, punctuation
- Broken or stale links
- Clarifying rewrites of a sentence or paragraph (keep the claim; sharpen the language)
- Better source citations for existing claims
- Accessibility fixes (alt text, semantic HTML, color contrast)
- Small visual/CSS polish that fits the existing aesthetic

For anything beyond that — open an Issue first.

## What belongs in an Issue (before you write code)

- Reframing a section's argument
- Proposing a new pullquote or figure
- Adding a new source to Further Reading
- Questioning a specific claim in an axiom
- Structural/architectural changes to the page
- Anything you're not sure about

Issues are cheap. Draft PRs that get closed are expensive. Open the Issue first.

## How to write the PR

1. Fork the repo and create a branch named after what you're changing (e.g. `fix-axiom-ii-typo`, `sharpen-telos-paragraph`).
2. Make the edit. Keep the diff small and focused.
3. If the change is substantive enough to be worth logging, **add a Revisions entry** at the bottom of `index.html` with today's date, a short name for the pass, and a one-paragraph description of what changed and why. Follow the existing format.
4. Preview locally: `python3 -m http.server 8000` and open http://localhost:8000.
5. Open the PR with:
   - **A one-sentence summary** of what changes
   - **Which axiom/section** the change touches
   - **Why** — what problem the current text has, or what the edit clarifies
6. Netlify will build a deploy preview on your PR so you (and reviewers) can see the rendered essay at a unique URL before merging.

## Style notes

- Prose is in `index.html`. There is no template system or content layer — you edit HTML directly.
- Semantic classes matter: `.pullquote`, `.attrib`, `.axiom-label`, `.numeral`, etc. Match existing patterns.
- Don't add build tools, frameworks, or package managers. This is deliberately a single HTML file.
- Don't restyle for its own sake. The visual language (Fraunces serif, JetBrains Mono, orange/amber/cyan palette, military-terminal hero) is load-bearing for the stance the document takes.

## Code of conduct

Disagree with the argument if you like; don't be a jerk about it. PRs and Issues that attack people rather than claims will be closed without discussion.
