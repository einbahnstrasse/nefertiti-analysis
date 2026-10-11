# Nefertiti: Interaction at Three Scales — version 2

Analysis of the Miles Davis Quintet’s “Nefertiti” (1967), with timestamp-linked Mermaid graphs at 3 scales, listening observations, scholarly citations, and downloadable materials exploring recursive ensemble interaction.

Complete webpage and analytical materials, October 11, 2026.

## Open locally

Open index.html, keeping mermaid.min.js beside it. Or open Nefertiti-Complete-Offline.html, a self-contained edition. Both display all six diagrams and source code without an internet connection. Video and source links require internet access. If clipboard access is blocked locally, select the Mermaid code directly.

Click a timestamped graph node to open the assigned YouTube video in a new tab at that time. Keyboard users can tab to these links. Nodes without a verified timestamp remain unlinked. Mermaid code itself has no click directives: the webpage adds SVG links using the per-graph links metadata in graphs.json. node-links.json also exports that mapping.

## GitHub Pages: simplest setup

1. Create a repository (a public repository works with GitHub Free).
2. Unzip Nefertiti-All-Materials-v2.zip.
3. Upload the CONTENTS of the extracted folder to the repository root, so index.html is directly beside README.md and mermaid.min.js. Do not upload the ZIP itself or put everything inside another enclosing folder.
4. Commit the files to main.
5. Open repository Settings > Pages.
6. Under Build and deployment, choose Deploy from a branch.
7. Choose main and / (root), then Save.
8. Use the Pages URL shown by GitHub after deployment, typically https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/.

No npm installation, framework build or custom GitHub Actions workflow is needed. All asset links are relative, so a project repository path works. The empty .nojekyll file bypasses Jekyll processing. Keep it when uploading; some file pickers hide dotfiles.

Alternative: put ALL these files in a folder named docs and choose main /docs in Pages settings. An arbitrary folder named website is not one of the branch-publishing folder choices; the previous package required moving its contents to the root or docs.

Official instructions:
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## Files

- index.html: GitHub Pages entry point, containing prose, citations, embedded analytical data and application code. Its styling comes from website.css.
- mermaid.min.js: bundled Mermaid 11.12.0 renderer; retain beside index.html.
- fonts/: self-hosted Crimson Pro variable webfonts (roman and italic) with their SIL Open Font License; retain beside index.html. Pages without this folder fall back to Georgia.
- Nefertiti-Complete-Offline.html: single-file edition, with renderer and data-download payloads embedded.
- Nefertiti-Analysis-and-Code.md: all prose, six diagrams as Mermaid code, observation table and bibliography.
- mermaid/: individual .mmd files and annotated graph documents; paste one .mmd at a time into Mermaid Live Editor.
- nefertiti-graphs.mmd: combined multi-graph source; split into individual diagrams for single-diagram editors.
- Mermaid-Graphs.zip: individual Mermaid materials packaged separately.
- Observations.csv: 32 observations for Excel or Sheets.
- observations.json and Observations.json: identical observation data, retained to support the original page links and standalone exports.
- graphs.json and Graphs.json: identical graph data, including explanatory prose, citations and node links.
- node-links.json: graph-node IDs mapped to YouTube timestamps and URLs.
- Sources-and-Citations.md: Chicago-style bibliography.
- website.css: the stylesheet for index.html, including the Crimson Pro font setup; retain beside index.html. Nefertiti-Complete-Offline.html embeds its own copy.
- website.js: extracted page script for editing; index.html and the offline edition embed it.
- MERMAID-LICENSE.txt: renderer license.

JSON files are exported copies. The current page embeds its data, so editing only a JSON file does not update index.html. To revise the page, edit its embedded graphs or rows arrays and the relevant prose, and update the exported copies to match.

## Evidence

The three zoom levels are performance, passage and local exchange. All timed links use Louis Goldford's assigned YouTube recording. Literature events without matched times remain pending. Solid arrows show sequence or structure; dashed arrows propose response or feedback. Original source articles and recording audio are referenced, not bundled. Graph syntax, data, search, scale filters and SVG link behavior were checked; full browser visual verification remains outstanding.

## License

© 2026 Louis Goldford. LICENSE is the authoritative text; in summary:

- Text, analysis, graphs and data (the prose, diagrams, observation ledger, notes and exported data files): all rights reserved. Students and educators may reproduce the graphs for coursework and teaching with citation. For any other reprinting or adaptation, please ask for permission.
- Code and website (HTML structure, website.css, website.js): MIT License; see LICENSE.
- Third-party components: the Mermaid renderer (mermaid.min.js, also embedded in Nefertiti-Complete-Offline.html) is © Knut Sveidqvist under the MIT License; see MERMAID-LICENSE.txt. The Crimson Pro fonts in fonts/ are © The Crimson Pro Project Authors under the SIL Open Font License 1.1; see fonts/OFL.txt.

Suggested citation: Goldford, Louis. “Nefertiti: Interaction at Three Scales.” Last modified October 11, 2026. https://einbahnstrasse.github.io/nefertiti-analysis/. Use the “Last modified” date shown on the page.
