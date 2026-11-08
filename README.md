# Whistling Hilltop Homestead Website

A small Jekyll website hosted with GitHub Pages. The pages use a simple shared layout and stylesheet, so you can change the homestead's text, colors, and navigation without needing a web framework.

## Where to make changes

| To change… | Edit this file | What to look for |
| --- | --- | --- |
| Homepage headline, welcome text, About section, and Journal teaser | `index.html` | Edit the visible text inside the corresponding HTML tags. Comments in the file label each section. |
| Browser tab title for the homepage | `index.html` | Change `title: Welcome` in the YAML block at the very top. |
| Site name and journal post URL pattern | `_config.yml` | Change `name` for the site name. `permalink` controls URLs for Jekyll posts. |
| Header links and footer text, shown on every page | `_layouts/default.html` | Edit the navigation list or footer paragraph. Keep the `id` fragments (`#homestead`, `#journal`) in sync with matching section IDs in `index.html`. |
| Page description for search engines | `_layouts/default.html` | Edit the `meta name="description"` content. |
| Colors, fonts, sizes, spacing, borders, and mobile layout | `css/main.css` | Change the `:root` color variables first; comments mark each style section. |

## Editing the homepage

1. Open `index.html` in the repository.
2. Replace the sample wording with your own homestead details. The first section is the large welcome area, the second is the About section, and the third is the Journal teaser.
3. Keep the HTML tags and section IDs (`homestead` and `journal`) unless you also update links that refer to them.
4. Commit your changes. GitHub Pages will rebuild the site automatically if Pages is enabled for this repository.

## Changing the look

At the top of `css/main.css`, the `:root` variables define the palette:

- `--ink`: main text color
- `--muted`: supporting text color
- `--sage`: links and accent color
- `--paper`: page background
- `--line`: divider and border color

Colors can be written as hex values, such as `#66745a`. Other CSS sections are labeled with comments. The final `@media (max-width: 700px)` section controls the phone layout.

## Site structure

- `_config.yml` — Jekyll site name and publishing settings.
- `_layouts/default.html` — shared HTML shell, navigation, and footer.
- `index.html` — homepage content.
- `css/main.css` — all visual styling.
- `README.md` — this editing guide.

## Publishing

In the repository, open **Settings → Pages** and choose the `main` branch and `/ (root)` as the publishing source. Once enabled, GitHub Pages publishes the site and rebuilds it after commits to `main`.
