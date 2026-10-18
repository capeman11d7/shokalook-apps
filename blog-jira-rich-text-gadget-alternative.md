# Rich text on Jira dashboards: alternatives to the Atlassian Labs Rich Text Gadget (2026)

_By Shokalook Apps, the maker of Rendermark for Jira. Updated October 18, 2026. Marketplace figures were checked on October 16, 2026._

**Short answer:** To put formatted notes, announcements, tables or checklists on a Jira Cloud dashboard, you need a text gadget app. The free Atlassian Labs "Rich Text Gadget for Jira" is the most installed, but it is unsupported, and reviews mention timeouts, a serif font that looks out of place and no dark mode. **Rendermark: Rich Text & Markdown Gadget for Jira** renders Markdown in your browser (so no server timeouts), matches Jira's look in light and dark mode, and is free for up to 10 users.

## The options

| Gadget | Maker | Installs | Rating | Price, 11–100 users |
|---|---|---|---|---|
| Rich Text Gadget for Jira | Atlassian Labs (unsupported) | 7,483 | 3.3★ | Free |
| Rich Text Editor: Notes Gadget for Jira | DarkSky | 303 or fewer | — | $0.49/user/month |
| Rich Text for Jira Dashboards | sellerkit | 303 or fewer | — | $0.45/user/month |
| Markdown for Jira | Capable | — | — | $0.75/user/month |
| **Rendermark: Rich Text & Markdown Gadget** | Shokalook Apps | new | new | **Free to 10 users, then $0.25/user/month** |

Install counts and ratings change. Check the Atlassian Marketplace for current numbers.

## When to choose each

- **Atlassian Labs gadget:** free, and fine if a plain note is enough and you can live without support or dark mode.
- **DarkSky or sellerkit:** choose these if you want a visual (WYSIWYG) editor instead of Markdown.
- **Rendermark:** choose it for Markdown with live preview, callout panels, tables, code and diagrams that look native in Jira, at about half the price of the paid rich-text gadgets.

## What Rendermark for Jira does

- **Headings, links, lists, tables and checklists** (`- [x] done`).
- **Callout panels** in five colors using the GitHub syntax (`> [!INFO]`, `> [!WARNING]`, `> [!ERROR]`, `> [!SUCCESS]`, `> [!IMPORTANT]`).
- **Code** with syntax highlighting for about 35 languages, and **Mermaid diagrams** that load only when used.
- **A real editor:** live preview, an Insert menu for people who don't know Markdown, and the gadget title in the same dialog. Text pasted from ChatGPT or Claude renders as is.
- **Looks like Jira:** Jira's font, Atlassian design tokens, and full dark mode.
- **No timeouts:** content is stored in the gadget's configuration and rendered in the browser, so there's no server to wait for.
- **Respects permissions:** only dashboard editors can edit; everyone who can view the dashboard can read.

## Limits to know

- Markdown editing only (with an Insert menu); there's no WYSIWYG mode yet.
- Up to 30,000 characters per gadget. Images are shown by link, not uploaded.

## How to set it up

1. Install it from the [Atlassian Marketplace](https://marketplace.atlassian.com/apps/1625144740).
2. On a dashboard, choose **Add gadget** and search for "Rich Text & Markdown".
3. Write or paste your content, check the preview, add a title and save.

## FAQ

**How do I add formatted text to a Jira dashboard?**
Install a rich-text gadget app, add the gadget to a dashboard you can edit, and enter your content.

**Why does the old Rich Text gadget time out?**
Reviews of the Labs gadget report timeouts loading content. Rendermark avoids this design: it renders locally in your browser.

**Is there a dark-mode text gadget for Jira?**
Yes. Rendermark follows Jira's light or dark theme automatically.

**Does it work in Jira Service Management dashboards?**
Yes. It's a standard Jira Cloud dashboard gadget.

[Documentation](rendermark-jira-gadget-docs.html) · [Privacy policy](rendermark-jira-gadget-privacy.html) · [All articles](blog.html) · Support: rendermark.support@gmail.com
