# M2 Master

An account-free HKDSE Mathematics Extended Part Module 2 practice website.

- 15 teaching chapters and a supplementary prerequisite area.
- 77 English Concepts & Formulas pages with LaTeX, worked examples and self-checks.
- 2,473 questions, including 525 distinct questions imported from bk1.pdf.
- Multiple-choice marking, original question images, printed answer excerpts and device-local handwritten drafts.
- Responsive layouts, light/dark mode, locally bundled KaTeX and fonts.

## Hosting

GitHub Pages is enabled with GitHub Actions. The deployment workflow reads the source, runs content checks and publishes the static website. It cannot write repository contents. No ChatGPT account, OpenAI service or API key is required by visitors.

## Source archives

The three m2-master-part-*.zip files together contain the complete editable source and static assets, split to stay within browser upload limits. Extract all three into the same directory to restore content/, scripts/ and docs/. The deployment workflow performs this extraction automatically in its temporary build workspace.

After editing the restored source, run python3 scripts/build-content.py and node scripts/validate-content.cjs. Repackage the updated source archives to publish a new version. The workflow is in .github/workflows/deploy-pages.yml. The current deployment uses GitHub Actions, rather than branch-based /docs publishing.

## Privacy

MC attempts, bookmarks and reading markers use localStorage. Handwritten drafts and photos use IndexedDB. Answers are stored only in the current browser; there are no server uploads or cloud marking. Records are specific to the website origin and do not automatically transfer from the previous hosting domain. Preserve answer photos and export MC records before moving devices.

## Content attribution

The 15 chapters are teaching units, not an official HKEAA chapter list. Third-party papers and images remain the property of their authors, publishers and examination bodies. The bk1 compilation retains dse.life attribution. Printed answer excerpts are not represented as complete official marking schemes. No licence to third-party paper content is granted by this repository.
