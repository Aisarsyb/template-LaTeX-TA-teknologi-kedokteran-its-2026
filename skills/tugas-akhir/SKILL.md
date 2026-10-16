---
name: tugas-akhir
description: Create a Medical Technology ITS thesis project, write its proposal or thesis, or check its PDF.
---

# Medical Technology ITS thesis

Resolve `template/` relative to this SKILL.md; work in the user's workspace.

## Start a project

If a thesis project exists, use it. Otherwise, show the destination and obtain consent before copying `<skill-directory>/template/.` into an empty directory. Confirm `sempro.tex`, `buku-ta.tex`, `bab/`, and `pustaka/variables.tex` exist.

## Write

Identify requested section, study data, and sources in `pustaka/variables.tex`, `abstrak/`, `bab/`, and `pustaka/pustaka.bib`; chapters 1–3 serve both documents. For each Bab 1–5 being written or reviewed, read its matching `references/sistematika-penulisan-babN.md` first and follow its structure and criteria. Use `/scientific-writing` for scientific content. Ground every factual claim and citation in available evidence; flag missing facts instead of inventing results or references. Write from a medical perspective.

Apply these rules to thesis prose:
- Use technical terms familiar to general readers; explain terms needed for medical accuracy.
- Explain why a method fits the study and, where relevant, why alternatives were not chosen.
- Present scientific arguments mainly in connected paragraphs; use lists or numbering when they make steps, criteria, or comparisons clearer.
- Write natural, straightforward Indonesian for medical readers: state the point directly and explain its reason; trim ceremonial openings and repeated phrases. Keep established technical terms when translating them would obscure meaning.
- Italicize foreign words or phrases retained in Indonesian prose: `\emph{motion artifact}` in LaTeX or `*motion artifact*` in Markdown. Leave abbreviations, units, names, and Indonesian terms in regular type.
- Dont use emdash (---) (--) and ";"

## Check

After writing or editing thesis content, or when the user requests a review, audit, or check, identify the affected chapters (or the chapters the user names), their matching `references/sistematika-penulisan-babN.md` guides, and available study data and sources. Spawn two read-only subagents **in parallel**, each with only its own brief so their judgments remain independent:

- **Guide:** Read the matching `references/sistematika-penulisan-babN.md` files **relative to this SKILL.md** as the standards for each chapter's writing structure, and apply the thesis prose rules above. Compare every relevant criterion with the chapter and cite the guide file and section or the prose rule for each unmet criterion, alongside the chapter passage, reason, and needed correction. Use the manuscript's headings to locate passages, not as a substitute for the guides.
- **Evidence:** Use `/scientific-critical-thinking` to check whether sources, methods, and data support each substantive claim, especially clinical conclusions. Report unsupported claims with the passage, available or missing evidence, impact, and needed correction; distinguish unknown facts from demonstrated errors.

Give both agents the chapter paths and relevant sources; give the Guide agent the exact matching guide paths. Ask them to report only findings they can locate, or explicitly say none.

### Aggregate

Present the subagents' reports under separate `## Guide` and `## Evidence` headings, verbatim or lightly cleaned. Do not merge or rerank findings across axes. End with one line stating the finding count and most serious issue within each axis, if any; do not pick an overall winner. After writing or editing, resolve substantiated findings before completion and report gaps that require missing facts. For review-only requests, leave the manuscript unchanged.

Only after editing LaTeX files, build the requested document once from the project root: `latexmk -xelatex -halt-on-error sempro.tex` or `latexmk -xelatex -halt-on-error buku-ta.tex`. If the target is unspecified and shared files changed, build both. If `latexmk` is unavailable, follow the README's `xelatex`/`biber` sequence. Report errors, PDF path, edits, and facts needing confirmation; check official requirements and supervisor guidance before submission.
