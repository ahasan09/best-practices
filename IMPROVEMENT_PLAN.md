# Improvement Plan: best-practices

## Overview
Documentation-only repository for team development standards. Static Markdown files with no automation, versioning, or discoverability tooling.

## Improvements

### Structure & Navigation
- Add a root `README.md` (or `index.md`) as a table of contents linking to all guidelines documents
- Organize documents into categories: `git/`, `code-review/`, `testing/`, `deployment/`, etc.
- Add a CHANGELOG or version history to track when guidelines were updated and why

### Content Quality
- Review all existing guidelines for accuracy against current tool versions (e.g., ESLint config format changed significantly in v9)
- Add concrete code examples (`good` vs `bad`) alongside each rule
- Add rationale/motivation for each guideline — "why" helps teams apply rules in edge cases

### Tooling
- Add a Markdown linter (e.g., `markdownlint`) via pre-commit hook and GitHub Actions to enforce consistent formatting
- Add a link checker to detect broken internal or external links
- Add a static site generator (MkDocs with Material theme or Docusaurus) to publish the guidelines as a browsable site

### Collaboration
- Add a `CONTRIBUTING.md` explaining how team members can propose or update guidelines
- Add a GitHub Actions workflow to require at least one reviewer approval for any documentation change

### DevOps
- Deploy the generated site to GitHub Pages automatically on merge to `main`
