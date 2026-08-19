<img src="images/knight-logo.png" alt="KNIGHT logo" width="110" align="right">

# KNIGHT project site

Quarto website for the KNIGHT project -- knowledge-graph methods (KG
construction, GraphRAG, and agentic reasoning) for neuromorphic computing
co-design.

## Structure

- `index.qmd` -- Home / project overview
- `people.qmd` -- Team and collaborators
- `publications.qmd` -- Papers, preprints, and bibliography (`bib/refs.bib`)
- `software.qmd` -- Software artifacts (KG pipeline, GraphRAG layer, Streamlit app)
- `community.qmd` -- Talks, posters, and workshop activity
- `images/` -- Figures used across pages
- `papers/` -- Downloadable paper PDFs

## Local development

```bash
quarto preview      # live-reloading local preview
quarto render       # one-off build to docs/
```

## Deployment

This site publishes to the `gh-pages` branch of the GitHub repository.

Manual publish:

```bash
quarto publish gh-pages
```

Automated publish: `.github/workflows/publish.yml` rebuilds and redeploys
the site to `gh-pages` on every push to `main` via GitHub Actions.
