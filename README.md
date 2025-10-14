# Jeongyong's Homepage

This is the personal homepage of Jeongyong Yang (Seiryu Takahashi).

<p align="center">
  <a href="https://takahashi-seiryu.github.io" target="_blank">
    <img src="https://img.shields.io/badge/Website-takahashi--seiryu.github.io-blue" alt="Website">
  </a>
</p>

# Usage

## Local Development (Docker)

```bash
docker compose pull
docker compose up
```

Then visit `http://localhost:8080` in your browser. Stop the stack with `docker compose down` when you are done.

## Updating Content

**Home Page**

- Hero narrative and profile: `_pages/about.md`
- News items: `_news/` (each file is a post)
- Selected publications list: mark entries with `selected={true}` inside `_bibliography/papers.bib`

**Publications**

- BibTeX records: `_bibliography/papers.bib`
- Co-author metadata: `_data/coauthors.yml`
- Venue metadata: `_data/venues.yml`
- Preview images: `assets/img/publication_preview/`

**CV**

- Downloadable PDF file: configure `cv_pdf` in `_pages/cv.md`
- Interactive/web CV data: `assets/json/resume.json`

After Updating, use prettier:

```bash
$ npx prettier --write .
```
