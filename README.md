# Barlow Business — Publii theme

A Publii-first business theme for consulting firms and professional services websites. The design is inspired by the clean, configurable structure of Publii Technews and adapted for Barlow Consulting; homepage copy and sections remain editable in Publii rather than hard-coded in templates.

## Set up the business homepage

1. Create a Page named **Home** and use Publii’s Block editor to add the content: a short hero lead, an About section, a two-column capabilities/services section, optional project highlights, and a Contact section. Use headings, paragraphs, Columns, Group, Image, and Buttons blocks so all copy and images are editable in Publii.
2. In the page editor’s template selector, choose **Business homepage**. This presents the Publii page title/featured image as the hero and renders the page’s block content below it.
3. In **Site settings → Advanced options → SEO**, enable **Use a page as the frontpage** and select Home.
4. In **Theme → Basic settings**, upload the Barlow logo in **Site logo for header and footer**. The theme uses Publii’s `@website.logo` and `@website.logoSize` values; if no image is configured, it displays a simple text fallback.
5. Edit the **Main menu** and **Footer menu** in Publii’s Menus area. The theme renders those assigned Publii menus; it does not invent About/Capabilities/Contact links or static anchors.
6. Configure the header CTA, shared contact details, favicon, sidebar, and post listing controls in **Theme → Custom settings**.

## What the theme renders

- **Business homepage** (`page-business-home.hbs`): editable page title, optional featured image, and all Block editor HTML. No hard-coded service or marketing copy.
- **Default pages** (`page.hbs`): standard editable Publii pages, including featured image, author options, child pages, and custom HTML injection.
- **Posts listing** (`index.hbs`): configurable editorial/news cards; use a posts prefix if the business homepage should be separate from the blog.
- **Post page** (`post.hbs`): article metadata, featured image, author bio option, related/previous-next posts, and comments support.
- **Shared shell** (`partials/navbar.hbs`, `partials/footer.hbs`): Publii logo, assigned menus, optional search input, CTA, contact details, footer code, and Publii cookie footer.

## Logo note

Publii exposes a theme Basic Settings logo as `@website.logo`; the logo’s dimensions are in `@website.logoSize.width` and `.height`. Upload it in the theme’s Basic Settings (not just as a block image in the Home page). Both header and footer use this value.

## Theme assets

- `assets/css/style.css` is the stylesheet entry point loaded by Publii and imports `main.css`.
- `assets/css/main.css` provides the responsive business visual system and styles Block editor content.

