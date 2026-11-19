# Pro Idea Website — Development and Build Guide

**Repository:** ProIdeaCodeStudio/Pro-Idea  
**Website:** https://proideacodestudio.github.io/Pro-Idea/  
**Documentation basis:** Repository commit history inspected on 19 November 2026  
**Purpose:** Explain the website's evolution, its major parts, and the reasoning behind the current structure in a way that can be followed by a learner.

---

## 1. How to read this guide

This guide follows the repository history from the earliest visible website commit through the current multidisciplinary portfolio work. It groups closely related commits into development phases so the learning path is understandable rather than presenting dozens of isolated commit titles.

The chronology is based on commit messages and the repository's current files. Where a commit message is generic (for example, "Update Pro-Idea.html" or "Add files via upload"), the exact feature cannot reliably be inferred from the message alone. Those entries are described as incremental editing or asset updates, not as specific features.

This is an educational overview. It intentionally does not publish private configuration, credentials, access details, sensitive integration internals, or instructions that could weaken the site's security.

If a topic is marked **Contact the senior developer**, do not try to reverse-engineer or change it from this guide.

**Senior developer contact (email only):** Proidea2025@gmail.com

---

## 2. The website at a glance

The project began as a web presence for Pro Idea and developed through several stages into a portfolio. The current direction presents three distinct areas:

1. **Graphic design** — visual identity, promotional design and selected creative work.
2. **Web development** — front-end website capabilities and services offered.
3. **Electrical learning** — a carefully scoped record of foundational electrical training and technical development.

The website is a static, repository-hosted site. Its visible pages are built from HTML, styled with CSS, and use JavaScript for selected interactions. The public site is published through GitHub Pages.

### Main files and their roles

| File or folder | Role |
|---|---|
| `index.html` | Main portfolio homepage and navigation hub |
| `StyleSheet.css` | Main site-wide visual system and homepage styling |
| `BrandTokens.css` | Shared Ember palette, typography and design tokens |
| `Gallery.html` | Full graphic design portfolio gallery |
| `Gallery.css` | Gallery-specific styling layered on the shared brand system |
| `graphic-design.html` | Graphic design service information and selected work |
| `web-development.html` | Web development capabilities and service information |
| `electrical-installation.html` | Electrical training and technical learning information |
| `ServicePages.css` | Shared layout and styling for the discipline pages |
| `Graphics/` | Artwork displayed in the gallery and selected-work sections |
| Image and logo assets in the root | Brand marks and supporting visual assets |

A file's presence does not automatically mean it is used by every page. Each HTML document must link the stylesheets and assets it needs.

---

## 3. Development timeline from the commit history

### Phase 1 — First website foundation
**13–17 April 2026**

The earliest repository commit is dated 13 April 2026 and is titled **"first commit"**. The following commits show repeated edits to the original Pro-Idea page and its stylesheet.

The commit messages indicate an early cycle of:
- Creating the first page structure.
- Iterating on the page's HTML.
- Updating the stylesheet as the appearance developed.
- Refining the page through several small revisions.

Several commits in this early period have generic messages such as "describe your change". Their exact individual changes cannot be established from their titles alone.

**What to learn from this phase:** A website often starts as one HTML document and one stylesheet. The HTML establishes content and structure; CSS controls how that structure looks. Iteration is normal, but meaningful commit messages make the history easier to understand later.

### Phase 2 — Early page and visual refinements
**17 April – 10 May 2026**

The commit history records further HTML and stylesheet revisions, followed by additions and removals of early experimental pages and supporting materials.

The history includes:
- Further changes to the original page and stylesheet.
- Uploads of supporting files and visual assets.
- Experiments with additional pages and learning-resource sections.
- Removal of several temporary or superseded pages and folders.
- Changes to the original brand-kit and colour-system material.

The important lesson is that not every experiment becomes part of the final website. Removing an outdated page can be part of keeping a project understandable.

Some commits from this period relate to private application or service integrations. Their technical details are intentionally not reproduced here.

**Restricted area:** Contact the senior developer — Proidea2025@gmail.com

### Phase 3 — Portfolio structure and navigation
**13–14 May 2026**

The commit history shows a substantial round of work on the main portfolio structure.

Notable recorded changes include:
- Updating the stylesheet for the portfolio design system.
- Revising the page's metadata, navigation, content sections and footer.
- Renaming the original page to `index.html`, establishing the conventional homepage filename.
- Refining the navigation bar and its links.
- Updating links so that the portfolio points to `Gallery.html`.
- Adding a more developed header and introductory content to the gallery.

**What to learn from this phase:**
- `index.html` is a common default homepage filename for static websites.
- Navigation links connect separate pages and sections.
- A page should have a clear hierarchy: navigation, introduction, main content and footer.
- When a file is renamed, links pointing to the old filename may also need to be updated.

### Phase 4 — Responsive navigation and image experience
**14–15 May 2026**

The commit history records work on:
- Responsive navigation styles.
- A hamburger menu for smaller screens.
- Lazy loading for images.
- Image loading indicators.
- A network-related notice.
- Updates to gallery images and titles.

Lazy loading is a browser feature that allows images farther down a page to wait before loading until they are closer to the visible area. It can reduce the amount of content the browser needs to load immediately.

A loading indicator can communicate that an image is still being fetched. It should also disappear when an image finishes loading or fails.

**What to learn from this phase:** A gallery is not just a collection of image tags. It needs responsive layout, meaningful alternative text, sensible loading behaviour and a usable experience on touchscreens.

### Phase 5 — Gallery interaction and content updates
**15–18 June 2026**

The commit history records several gallery-focused changes:
- Updating gallery content, images and titles.
- Adding more team flyer designs.
- Correcting an image source typo.
- Correcting image tags and an icon type.
- Adding an image overlay and navigation buttons.
- Fixing a duplicate stylesheet link on the homepage.

An image overlay, often called a lightbox, lets a visitor view a selected image in a larger presentation without leaving the gallery. Previous and next controls allow movement between images.

**What to learn from this phase:** Interactive features have both a visual part and a behaviour part. The HTML supplies the controls and image elements, CSS presents the overlay, and JavaScript responds to user actions.

### Phase 6 — Logo asset update
**8 July 2026**

A commit records an update to the logo asset.

Brand assets should be referenced consistently. When an image filename changes, every page that uses that image must point to the correct filename. File paths and capitalisation matter, particularly on case-sensitive hosting systems.

### Phase 7 — Multidisciplinary portfolio expansion
**18 November 2026**

A commit titled **"Expand Pro Idea into a multidisciplinary portfolio"** records the addition of graphic design, web development and basic domestic electrical installation disciplines to the homepage, while preserving the Ember brand system and updating contact details.

This marked a shift from a graphic-design-centred portfolio to a broader presentation of different capabilities.

A key content distinction was established:
- Graphic design can show actual selected designs.
- Web development should explain the kinds of websites and front-end work that can be offered, rather than implying that every service description is a completed project.
- Electrical content should describe the user's actual training and learning scope accurately. It must not imply a professional licence or authorisation that has not been established.

### Phase 8 — Modern editorial redesign
**18 November 2026**

The commit titled **"Redesign portfolio with modern editorial visual direction"** records a visual redesign of the homepage.

Its commit message notes:
- An editorial, multidisciplinary homepage layout.
- A replacement of the homepage's previous styling direction.
- Retention of the Pro Idea studio wordmark.
- Preservation of artwork proportions in the project gallery.
- Cleanup of stylesheet design-system comments.

This phase changed the visual presentation. It also created an important maintenance requirement: pages that still used older CSS class names needed to be updated or given compatible page-specific styling.

### Phase 9 — Ember system restoration and dedicated discipline pages
**19 November 2026**

The commit titled **"Restore Ember system and add discipline pages"** records the recovery of the original Ember brand tokens and the addition of dedicated pages for the three disciplines.

The original palette is defined in `BrandTokens.css`:

| Token | Value | Intended role |
|---|---|---|
| Deep Ink | `#111008` | Main dark background |
| Ash | `#1E1B12` | Raised dark surfaces |
| Ember Fog | `#8A7A5A` | Muted labels and supporting details |
| Parchment | `#DDD0B3` | Secondary text |
| Warm White | `#F5EDD8` | Main light text |
| Burnt Ember | `#B5660F` | Darker amber interaction state |
| Amber | `#E8941A` | Primary accent |
| Ember Tint | `#F2B455` | Lighter accent |

The same file also defines the font families:
- Syne for display headings.
- Cormorant Garamond for accent typography.
- Plus Jakarta Sans for body text.
- DM Mono for labels and small technical details.

The commit history records the creation of:
- `ServicePages.css`
- `graphic-design.html`
- `web-development.html`
- `electrical-installation.html`

It also records updates to the homepage so the three disciplines lead to their dedicated pages.

### Phase 10 — Quality corrections and shared page refinement
**19 November 2026**

The latest merged quality pass records corrections to:
- Homepage markup and theme metadata.
- Main stylesheet token usage and text contrast.
- Shared service-page layout.
- Tablet navigation responsiveness.
- Graphic design service-before-work content order.
- Electrical training scope wording.
- Metadata and navigation semantics on the discipline pages.
- Stray literal escape characters and dark-section colour consistency.

The quality pass is recorded in the commit **"Fix Ember portfolio quality and service page hierarchy"**.

---

## 4. Understanding the front-end building blocks

### HTML — the structure

HTML describes what each part of a page is.

Examples:
- A heading identifies a page or section.
- A paragraph contains explanatory text.
- A navigation element groups links.
- An image element displays an artwork file.
- An article element groups one portfolio card.

HTML should describe the meaning of content, not carry the entire visual design through inline styling.

### CSS — the presentation

CSS controls:
- Colours.
- Typography.
- Spacing.
- Grid and flex layouts.
- Image proportions and cropping.
- Hover and focus states.
- Responsive changes for different screen widths.

The project uses a shared design system. The brand tokens provide the reusable values; page styles apply those values to specific components.

### JavaScript — interaction

JavaScript adds behaviour to the page. In the portfolio this includes interactions such as opening a mobile navigation menu, observing content as it enters the viewport, and operating the gallery image viewer.

A good interactive feature should also consider keyboard use, focus visibility and what happens when the user closes the interaction.

### Asset paths

An image reference such as:

`Graphics/MARCH.png`

means the browser looks for a folder named `Graphics` relative to the HTML page, then a file named `MARCH.png` inside it.

Keep the spelling, spaces, punctuation and capitalisation identical to the repository filename. A path that works on one local computer may fail after deployment if the case does not match.

---

## 5. How the current gallery is organised

The gallery preserves three content groups:

1. **Pre-rebranding designs** — earlier work, kept as part of the design journey.
2. **Post-rebranding designs** — work reflecting the later visual direction.
3. **IEEE R8 designs** — the client-approved collection identified in the page.

The gallery uses the artwork stored in the `Graphics/` folder. Each card groups an image with its category, title and (where supplied) a short description.

### Gallery stylesheet relationship

The gallery now loads two stylesheets:

1. `StyleSheet.css` — shared site styles and the main Ember system.
2. `Gallery.css` — gallery-specific layout, cards, navigation presentation, image viewer and responsive rules.

`Gallery.css` imports `BrandTokens.css` so the gallery uses the same palette and typography as the rest of the website.

This is intentional: shared tokens keep the brand consistent, while page-specific CSS avoids forcing every gallery detail into the homepage stylesheet.

### Image viewer behaviour

The gallery image viewer is designed to:
- Open when an artwork is selected.
- Show the selected image at a larger size.
- Move to the previous or next image.
- Close using the close control or Escape key.
- Support left and right arrow keys while open.
- Return keyboard focus to the image that opened it.

---

## 6. Safe maintenance workflow

Use this general learning workflow for ordinary presentation changes:

1. Identify the page or component that needs changing.
2. Find the relevant HTML file.
3. Identify the stylesheet linked by that page.
4. Check whether the desired styles belong in the shared stylesheet or the page-specific stylesheet.
5. Reuse the existing Ember variables instead of inventing new brand colours.
6. Make one coherent change at a time.
7. Check the page at desktop and mobile widths.
8. Check that image paths still work.
9. Test navigation, buttons, image viewer controls and keyboard focus.
10. Review the change before merging it into the published branch.

### Before changing a stylesheet

Ask:
- Is this stylesheet actually linked by the page?
- Does the selector in the CSS match the class or ID in the HTML?
- Is another stylesheet overriding the rule?
- Is the rule inside a media query that only applies at a certain screen width?
- Is the colour a brand token or a hardcoded value?
- Does the change affect other pages that share this stylesheet?

### Commit message practice

A useful commit message says what changed and why. For example:

- `Fix gallery card spacing on mobile`
- `Add keyboard controls to gallery lightbox`
- `Correct broken artwork image paths`
- `Improve contrast in gallery project captions`

Avoid generic messages such as `update`, `changes` or `final fix`. Clear messages make the development history much easier to study.

---

## 7. Topics intentionally withheld

This guide does not contain operational details for private integrations, authentication or account flows, private service configuration, credentials, access tokens, deployment permissions, database access, or other sensitive implementation details.

Where the repository history indicates that such work took place, this guide records only that a restricted technical area existed. It does not reproduce implementation steps, endpoint details, configuration values or access procedures.

For any such subject, use this instruction:

**Contact the senior developer.**  
**Email:** Proidea2025@gmail.com

Do not place credentials or private configuration in HTML, CSS, public documentation, screenshots, commit messages or public repository files.

---

## 8. Suggested learning sequence

If you are studying how this website was built, follow this order:

1. Read `index.html` to understand the homepage structure.
2. Read `BrandTokens.css` and identify how the Ember colours and fonts are named.
3. Read `StyleSheet.css` and connect its selectors to the homepage elements.
4. Read `Gallery.html` and identify the three gallery collections.
5. Read `Gallery.css` and connect its rules to the gallery's HTML classes.
6. Read `graphic-design.html`, `web-development.html` and `electrical-installation.html` to compare how each discipline is presented.
7. Read `ServicePages.css` to understand how common layouts are shared across those pages.
8. Use the commit timeline in this guide to understand why the site changed over time.

The aim is not to memorise every line. It is to understand how structure, styling, assets, interaction and version history work together to form a maintainable website.

---

## 9. Repository history references

The following commit links are the source records used to build this timeline:

- [First commit — 13 April 2026](https://github.com/ProIdeaCodeStudio/Pro-Idea/commit/95e4db7a123ee3479206e3e29f925e3e9aa6b0db)
- [Portfolio HTML structure and content — 13 May 2026](https://github.com/ProIdeaCodeStudio/Pro-Idea/commit/3144df0a197d646fe8d89547cd8130bb61e7bd4d)
- [Homepage filename and navigation refinements — 14 May 2026](https://github.com/ProIdeaCodeStudio/Pro-Idea/commit/a6ed6236abf058686c8b32b40d87e2d6acc9f653)
- [Responsive navigation and lazy loading — 14 May 2026](https://github.com/ProIdeaCodeStudio/Pro-Idea/commit/e2ebaf5cfc254328ff1293e66edc7260e4a4f47c)
- [Image overlay and gallery navigation — 17 June 2026](https://github.com/ProIdeaCodeStudio/Pro-Idea/commit/8e5b8471492742dc790a8a3182711a6af40a8872)
- [Logo asset update — 8 July 2026](https://github.com/ProIdeaCodeStudio/Pro-Idea/commit/c60c9a1628b527d8439196d877c0696c4902bc0a)
- [Multidisciplinary portfolio expansion — 18 November 2026](https://github.com/ProIdeaCodeStudio/Pro-Idea/commit/21ddcaa9f71b6fb09b283d7f5a93f18baf0c5b9e)
- [Modern editorial redesign — 18 November 2026](https://github.com/ProIdeaCodeStudio/Pro-Idea/commit/5c23288be07791c6f975a5d66781769ba2cc3500)
- [Ember restoration and discipline pages — 19 November 2026](https://github.com/ProIdeaCodeStudio/Pro-Idea/commit/b681586f625b373deffeb9d7aa3ea0b89a7dd69d)
- [Latest merged quality corrections — 19 November 2026](https://github.com/ProIdeaCodeStudio/Pro-Idea/commit/a8a7a95300dd2a8e993f4d9835bc83ad1ffe3fc1)

---

**End of guide**  
Pro Idea — Website Development Notes
