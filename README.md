# Om Prakash | Engineering portfolio

A personal site about my work on Microsoft account and billing experiences, my earlier engineering roles, and two projects: **Fitness Tracker** and **Connect2Donor**. The site is plain HTML, CSS, JavaScript, and SVG. There are no packages to install and no build step.

## Preview locally

Open `index.html` directly, or run this command from the repository root with Python 3:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Visit [localhost:8000](http://127.0.0.1:8000/). Press `Ctrl+C` to stop the server.

## Explore the site

- **Hero:** Drag or tap the falling skill tiles. The orange sun/moon switch changes the theme and remembers the choice on this browser. To preview a specific palette, append `?scoutTheme=light` or `?scoutTheme=dark` to the URL.
- **Experience:** The Microsoft card starts in focus. Hover another card, tap it, or tab to its highlights to bring it into focus.
- **Contact:** Draw on the sketchboard with a mouse, touch, or arrow keys; drawings stay in the current page. The illustrated tabby follows the pointer, and the circular email link opens a mail draft.

The site respects the system's reduced-motion setting. Without JavaScript, the résumé content, project descriptions, expandable highlights, and contact links remain available.

## Edit the portfolio

| File | What to change |
| --- | --- |
| [`index.html`](index.html) | Experience, projects, skills, contact links, theme colors, and interactions. Styles and scripts are inline. |
| [`assets/portrait.svg`](assets/portrait.svg) | The illustrated portrait used in the hero and its blurred background. To use a photo instead, add it under `assets/` and change `--portrait` in `index.html`. |

Before publishing, confirm the LinkedIn link in the footer: the résumé supplied the handle `om-prakash`, not a full URL. The site does not include a phone number or home address.

## Publish with GitHub Pages

1. Put `index.html`, `assets/`, and `.nojekyll` at the root of the branch you want to publish.
2. In the repository, open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select that branch and **/(root)**, then **Save**. When deployment finishes, use **Visit site** on the Pages settings page.

`.nojekyll` tells Pages to serve the files as written. Any other static host can serve the same files; keep `assets/` next to `index.html` so the portrait loads.

## Design references

The original artwork and interactions draw inspiration from [Bruno Simon](https://bruno-simon.com/), [Adrian Hajdin's 3D developer portfolio](https://github.com/adrianhajdin/project_3D_developer_portfolio), and [Arjun R](https://arjunr.dev/).