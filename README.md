# Biostatistics for Biomedical Research — web mirror

A static mirror of **Biostatistics for Biomedical Research (BBR)** by
**Frank E. Harrell Jr.**, originally published at <https://hbiostat.org/bbr/>.

The book is reproduced page for page: 25 chapters and appendices, every figure,
interactive Plotly widget, code block, table and cross-reference.

- Original: <https://hbiostat.org/bbr/>
- Author: Frank E. Harrell Jr. (Vanderbilt University)
- Licence: [GPL-3.0](LICENSE)

## What changed

The mirror is the original HTML, not a re-render. Two mechanical changes only:

1. Quarto emits extensionless links (`/bbr/r`), which the original Netlify host
   resolves to `r.html` but GitHub Pages does not. Every internal link was
   rewritten to the corresponding local `.html` file.
2. The Google Analytics snippet was removed (it reported to the original
   site's property).

Text, code, figures, styling, navigation and the search index are unchanged.

## Structure

```
index.html          # Preface
r.html … alpha.html # chapters, at the site root
figures.html        # list of figures
references.html     # annotated references
*_files/            # per-chapter figure assets
images/             # shared images
site_libs/          # Bootstrap, Quarto JS, Plotly, search
h.css               # book stylesheet
search.json         # full-text search index
```

Serve locally with any static server:

```bash
python3 -m http.server 8000
```
