# Md. Arifur Rahman — Personal Academic Website (Lab Notebook Theme)

Single-page portfolio for Md. Arifur Rahman, veterinarian and researcher in poultry disease diagnostics, veterinary microbiology and molecular diagnostics (Dhaka, Bangladesh).

## Theme

A lab-notebook look on graph paper, with a fixed sidebar and hard-edged "offset shadow" cards.

- **Light mode:** cream paper, black ink, vermilion accent.
- **Dark mode:** blueprint navy with cyan and amber accents.
- The theme follows the visitor's system setting, and the **LIGHT / DARK** button in the sidebar switches it. The choice is remembered in the browser.

No build step and no dependencies.

## Social links with logos

The sidebar and the Contact section show: ORCID, LinkedIn, Google Scholar, ResearchGate, Scopus, Email and Phone. Each has its brand logo as an inline SVG.

The logos are simplified brand marks drawn in the page, so the site works offline with no image files. To use an official logo, replace the matching `<symbol id="i-...">` block at the top of `index.html` with the organisation's official SVG.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The whole site: HTML, CSS and JavaScript |
| `portrait.jpg` | Profile photo shown in the sidebar |
| `README.md` | This file |

## Deploy on GitHub Pages

1. Create a public repository named `<your-github-username>.github.io`.
2. Upload `index.html`, `portrait.jpg` and `README.md` to the repository root.
3. Go to **Settings → Pages**, set **Source** to **Deploy from a branch**, choose `main` and `/ (root)`, then save.
4. The site goes live at `https://<your-github-username>.github.io` after a minute or two.

To preview locally, run `python3 -m http.server 8000` in the folder and open `http://localhost:8000`.

## Customising

- **Profile links:** edit the `LINKS` array at the top of the script. The ORCID, Scopus, email and phone links are real. The LinkedIn, Google Scholar and ResearchGate links are search links, so replace each `u:` value with your actual profile URL.
- **Publication links:** every entry opens a Google Scholar search for its title. In the `PUBS` array, add `url:"https://doi.org/..."` to an entry to link directly to the paper.
- **Skills and interests:** edit the `SK` object and `INT` array in the script.
- **Education, experience, awards:** plain HTML sections in `index.html`.
- **Colours:** change the CSS variables at the top of the `<style>` block. `:root` holds light mode and `:root[data-theme=dark]` holds dark mode.
- **CV download:** upload `cv.pdf` to the repository and add `<a class="btn" href="cv.pdf" download>CV ↓</a>` next to the hero buttons.

## Notes

- The page respects `prefers-reduced-motion`.
- Referee details from the CV are intentionally not published.
- Manuscripts marked "Under review" are not published papers.

## License

© Md. Arifur Rahman. All rights reserved. Please do not reuse the photo or text without permission.
