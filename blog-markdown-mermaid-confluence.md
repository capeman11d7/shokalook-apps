# How to render Markdown, Mermaid diagrams and code in Confluence Cloud (2026 comparison)

_By Shokalook Apps, the maker of Rendermark. Updated October 18, 2026. Marketplace install counts, ratings and prices were checked on October 15–16, 2026._

**Short answer:** Confluence Cloud does not render Markdown or Mermaid on its own. You need a Marketplace app. If you only need diagrams, a dedicated Mermaid app works. If your team pastes output from ChatGPT, Claude or Copilot, which mixes Markdown, tables, code and diagrams in one answer, **Rendermark: Markdown, Mermaid & Code for Confluence** renders all of it in one macro, with a live preview, PDF/Word export and dark mode. It is free for up to 10 users.

## Why this keeps coming up

AI assistants answer in Markdown. A design doc from Claude or ChatGPT usually has headings, a table, a code block and a Mermaid diagram. Confluence's editor turns that into plain text, so teams either reformat by hand or install separate Markdown, Mermaid and code macros.

## The options

| App | Maker | Installs | Rating | Price, 11–100 users | What it covers |
|---|---|---|---|---|---|
| Render Markdown | Atlassian Labs (unsupported) | 3,852 | 3.5★ | Free | Markdown only; last updated 2021 |
| Mermaid diagrams viewer | Atlassian Labs (unsupported) | 7,615 | 3.0★ | Free | Mermaid only |
| Better Code Macro | Atlassian Labs (unsupported) | 2,717 | 3.1★ | Free | Code only |
| Just Add+ | Modus | about 8,100 | 4.2★ | $0.50/user/month | Many formats (Markdown, diagrams, more) |
| Stratus Mermaid | Stratus | about 6,300 | 4.0★ | $0.40/user/month | Mermaid diagrams |
| **Rendermark** | Shokalook Apps | new | new | **Free to 10 users, then $0.45/user/month** | Markdown + Mermaid + code in one macro |

Figures come from the Atlassian Marketplace. Install counts include inactive sites, and ratings change, so check the listings for current numbers.

## When to choose each

- **Free Atlassian Labs macros:** fine for occasional use, if you accept that Atlassian labels them unsupported. Reviews have reported broken blocks after updates and no recent fixes.
- **Just Add+:** a good pick if you also need to embed other formats (it covers more than Markdown and Mermaid). It has a long track record.
- **Stratus Mermaid:** a good pick if diagrams are all you need.
- **Rendermark:** best when content arrives as mixed Markdown from AI tools or from GitHub READMEs, and you want one macro, a live preview and clean exports.

## What Rendermark does

- **One macro for everything:** GitHub-flavored Markdown (headings, tables, task lists, links), Mermaid diagrams (flowchart, sequence, class, state, ER, Gantt, pie, mindmap, timeline) and syntax-highlighted code in about 35 languages.
- **Paste AI output as is.** A ` ```mermaid ` block or a bare diagram both render.
- **Live preview editor,** with diagram errors that point to the broken line.
- **PDF and Word export** that keeps your text and tables as real Confluence content.
- **Light and dark mode** following the Confluence theme.
- **Safe and private:** HTML is sanitized, Mermaid runs in strict mode, the app requests no API scopes and has no servers of its own. It runs entirely on Atlassian Forge.

## Limits to know

- Diagrams export as their source text in PDF, not as images.
- It is a new app, so it has no reviews yet.

## How to set it up

1. Install **Rendermark** from the [Atlassian Marketplace](https://marketplace.atlassian.com/apps/3835433509).
2. Edit a page, type `/Rendermark`, and insert the macro.
3. Paste your Markdown, diagram or code, check the preview, and save.

## FAQ

**Does Confluence Cloud support Markdown natively?**
The editor accepts some Markdown shortcuts while you type, but pasted Markdown documents, tables and Mermaid diagrams don't render. You need a macro app.

**How do I add a Mermaid diagram to Confluence?**
Install a Mermaid-capable app (Rendermark, Stratus Mermaid, Just Add+ or the Labs viewer), insert its macro, and paste the diagram code.

**Can I paste ChatGPT or Claude output into Confluence with formatting?**
Yes, with a Markdown macro. Rendermark is built for this: paste the whole answer, including code blocks and diagrams.

**Is there a free option?**
Rendermark is free for sites with up to 10 users. The Atlassian Labs macros are free but unsupported.

**Does my content leave Atlassian?**
Not with Rendermark: it runs on Atlassian Forge with no outside servers and no tracking.

[Rendermark documentation](rendermark-docs.html) · [Privacy policy](rendermark-privacy.html) · [All articles](blog.html) · Support: rendermark.support@gmail.com
