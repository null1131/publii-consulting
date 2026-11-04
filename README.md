# Barlow Business — Publii theme

A Publii-first business theme for consulting firms and professional services sites. Homepage copy and sections are authored in Publii, not embedded in the theme templates.

## Build your homepage in Publii

1. Create a **Page** in Publii and edit it with the **Block editor**. Use normal headings, paragraphs, images, columns, buttons, lists, and other blocks to create the hero, about, services, testimonials, and contact sections you need.
2. In **Site settings → Advanced options → SEO**, enable **Use a page as the frontpage** and choose that page. Publii will render the selected page through `page.hbs`; the theme outputs its editable body with `{{{text}}}`.
3. Build your navigation in Publii’s **Menus** settings and assign it to Main menu and, optionally, Footer menu.
4. Configure shared details in **Theme → Custom settings**: header CTA, contact email/phone/location, footer note, blog sidebar, and font size. Set the site name and logo in Publii’s site/theme settings.
5. Create ordinary pages such as About, Services, and Contact in Pages. Their content uses the same block editor and business-style page layout.

## Posts and news

When the site is using a posts-listing homepage instead of a static frontpage, `index.hbs` displays recent posts. You can also set a posts prefix in Publii to keep news separate from a page-based homepage. Post titles, featured images, excerpts, and article bodies remain editable in Publii.

## Theme structure

- `page.hbs` — editable page and selected static-frontpage layout.
- `index.hbs` — editable Publii posts listing, with latest posts and pagination.
- `post.hbs` — individual post layout.
- `partials/navbar.hbs` / `partials/footer.hbs` — Publii-managed menus and configurable shared details.
- `assets/css/main.css` — responsive business styling for Publii content and editor-generated blocks.

## Theme development

The theme retains Publii’s standard templates, responsive image support, search/comments integrations, page and tag/author support, and custom HTML injection points. For developer details, see [Publii’s theme documentation](https://getpublii.com/dev/).
