# Om Prakash | Engineering portfolio

A personal site about my work on Microsoft account and billing experiences, my earlier engineering roles, and two projects: **Fitness Tracker** and **Connect2Donor**. The site is plain HTML, CSS, JavaScript, and SVG. There are no packages to install and no build step.

## Preview locally

Open `index.html` directly, or run this command from the repository root with Python 3:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Visit [localhost:8000](http://127.0.0.1:8000/). Press `Ctrl+C` to stop the server.

## Explore the site

- **Hero:** Drag or tap the falling skill tiles; their glossy highlight stays on the screen-facing top edge as they tumble. The sun/moon switch below the heading toggles between light and midnight-blue themes and remembers the choice on this browser. To preview a specific palette, append `?scoutTheme=light` or `?scoutTheme=dark` to the URL.
- **Experience:** The Microsoft card starts in focus. Hover another card, tap it, or tab to its highlights to bring it into focus. On hover, the card lifts without resizing the text or shifting its neighbors. Reduced motion keeps it stationary.
- **Resume:** Choose Resume in the navigation for a short career summary and a link to the full document on Google Drive. The document’s visibility is controlled by its Drive sharing settings.
- **Contact:** Draw on the sketchboard with a mouse, touch, or arrow keys; drawings stay in the current page. The illustrated tabby follows the pointer, and the circular email link opens a mail draft.

The navbar uses frosted acrylic in both themes. In dark mode, a translucent smoke tint lets scrolling content show through the blur while the links stay sharp. The navbar stays opaque when reduced transparency is requested or backdrop blur is unavailable. The site also respects the system's reduced-motion setting. Without JavaScript, the resume content, project descriptions, expandable highlights, and contact links remain available.

## Edit the portfolio

| File | What to change |
| --- | --- |
| [`index.html`](index.html) | Experience, projects, skills, contact links, theme colors, and interactions. Styles and scripts are inline. |
| [`assets/portrait.jpg`](assets/portrait.jpg) | Om's photo, used in the hero and its blurred background. Replace it here or update `--portrait` in `index.html` to point to a different file. |

Before publishing, confirm the LinkedIn link in the footer: the resume supplied the handle `om-prakash`, not a full URL. The site does not include a phone number or home address.

## Publish with GitHub Pages

1. Put `index.html`, `assets/`, and `.nojekyll` at the root of the branch you want to publish.
2. In the repository, open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select that branch and **/(root)**, then **Save**. When deployment finishes, use **Visit site** on the Pages settings page.

`.nojekyll` tells Pages to serve the files as written. Any other static host can serve the same files; keep `assets/` next to `index.html` so the portrait loads.

## Design references

The original artwork and interactions draw inspiration from [Bruno Simon](https://bruno-simon.com/), [Adrian Hajdin's 3D developer portfolio](https://github.com/adrianhajdin/project_3D_developer_portfolio), and [Arjun R](https://arjunr.dev/).

The employer icons are the site icons published by [Microsoft](https://www.microsoft.com/), [InsuranceDekho](https://www.insurancedekho.com/), and [Cadence PCB Resources](https://resources.pcb.cadence.com/). The footer uses [Bootstrap Icons](https://icons.getbootstrap.com/) under the [MIT license](assets/bootstrap-icons-LICENSE.txt). All six icons are served locally.