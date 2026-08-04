# Portfolio site

A single-page operator portfolio for a Revenue Operations / Chief of Staff leader, deployed
as a static site on GitHub Pages. Business and financial outcomes lead; the shipped code and
frameworks are the proof points.

## Files
- `index.html`: the one-page portfolio (self-contained; fonts load from Google Fonts, with system fallbacks)
- `local-slm.html`: the "Local SLM Evaluation for RevOps" case-study page
- `local-slm-assessment.pdf`: downloadable full assessment for the SLM case study
- `meddpicc-deal-scoring-framework.pdf`: downloadable, anonymized sample of the deal-scoring rubric behind the Intelligent Forecast workflow
- `workflow-prioritization-matrix.pdf`: downloadable, anonymized sample of how dozens of manual workflows get scored and sequenced into a 90-day roadmap
- `frameworks/`: the HTML sources the two framework PDFs are rendered from
- `Stephen_Jang_Portfolio.png`: link-preview image (Open Graph / Twitter card)
- `.nojekyll`: tells GitHub Pages to serve files as-is (no Jekyll build)

## Downloadable artifacts
Two anonymized operational frameworks are linked directly from the page so a recruiter or
hiring manager can open a tangible artifact, not just a code demo:

- **MEDDPICC Deal-Scoring Framework**, linked from the *Intelligent Forecast* project.
- **Workflow Prioritization Matrix**, linked from the *GTM Architecture* section.

All thresholds and scores in them are illustrative samples, not real customer data.

### Regenerating the framework PDFs
Each PDF is rendered from a self-contained HTML file in `frameworks/` via headless Chromium:

```
chromium --headless --no-pdf-header-footer \
  --print-to-pdf=meddpicc-deal-scoring-framework.pdf \
  frameworks/meddpicc-deal-scoring-framework.html
```

Edit the HTML source and re-render if a framework changes. Each is laid out to fit on a
single Letter page.

## The 90-day plan stays private
The full 90-day implementation plan is **not** published. The sticky "Get the 90-day plan"
banner and the closing call-to-action open a pre-filled email (native mail client, with a
Gmail-compose fallback) so interested people reach out directly. Send the plan manually in
reply.
