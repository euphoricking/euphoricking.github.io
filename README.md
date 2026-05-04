# Ekata Leo Oni — GIS ePortfolio

Professional GitHub Pages + Jekyll ePortfolio for MSc Applied Geoinformatics, GIS, WebGIS, spatial databases, GeoAI, BI, and data engineering.

## 1. What to edit first

Open `_config.yml` and change:

```yml
email: "your.email@example.com"
url: "https://your-github-username.github.io"
author:
  linkedin: "https://www.linkedin.com/in/your-linkedin"
  github: "https://github.com/your-github-username"
```

If this site is deployed as a project repository, for example:

```text
https://your-github-username.github.io/eportfolio/
```

then set:

```yml
baseurl: "/eportfolio"
```

If it is deployed as your main GitHub Pages site:

```text
https://your-github-username.github.io/
```

then keep:

```yml
baseurl: ""
```

## 2. Add your own images

Replace the placeholder SVG files in:

```text
assets/img/projects/
```

Use screenshots of your maps, dashboards, charts, thesis workflow diagrams, and project outputs.

## 3. Add your CV

Place your CV PDF here:

```text
assets/files/Ekata_Leo_Oni_CV.pdf
```

The CV page already links to this file.



## 3b. Add your profile photo

The homepage currently uses this placeholder:

```text
assets/img/profile-placeholder.svg
```

To use your real photo, upload your image as:

```text
assets/img/profile.jpg
```

Then open `index.md` and change:

```html
<img src="{{ '/assets/img/profile-placeholder.svg' | relative_url }}" alt="Profile placeholder" class="profile-image">
```

to:

```html
<img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Ekata Leo Oni" class="profile-image">
```

## 4. Add or edit projects

Each project is stored in:

```text
_projects/
```

To create a new project, duplicate one of the existing `.md` files and edit the front matter:

```yml
title:
category:
summary:
tools:
status:
period:
featured:
image:
```

Valid portfolio categories used by the portfolio page:

- MSc Thesis & Research
- WebGIS & Dashboards
- Spatial Databases & SDI
- GeoAI & Remote Sensing
- Data Engineering & BI

## 5. Run locally

Install Ruby and Bundler, then run:

```bash
bundle install
bundle exec jekyll serve
```

Open:

```text
http://localhost:4000
```

## 6. Deploy on GitHub Pages

1. Create a GitHub repository, for example `eportfolio`.
2. Upload all files from this folder.
3. Go to repository **Settings**.
4. Go to **Pages**.
5. Under **Build and deployment**, select:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
6. Save.
7. Wait for GitHub Pages to build the site.

Your site will be available at:

```text
https://your-github-username.github.io/eportfolio/
```

## 7. Recommended submission note

When submitting the ePortfolio URL, use a short message:

> Dear [Lecturer/Supervisor],
>
> Please find below the URL to my MSc Applied Geoinformatics ePortfolio:
>
> [Insert URL]
>
> The portfolio documents selected academic projects, MSc thesis work, WebGIS outputs, spatial database work, and professional data-related skills developed during the programme.
>
> Kind regards,  
> Ekata Leo Oni


## Project update included

This package includes six refined portfolio projects: MSc Thesis, PowGenAUS, Explore Salzburg WebGIS, Central Europe Employment SDI WebGIS, Spatial Database Backend for a City Festival WebGIS, and BlockPulse. Project screenshots and selected downloadable reports are stored under `assets/img/projects/` and `assets/files/projects/`.
