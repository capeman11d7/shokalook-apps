# Rendermark: Markdown, Mermaid & Code for Confluence — Documentation

Rendermark is a Confluence Cloud macro that renders Markdown, Mermaid diagrams and syntax-highlighted code, for example output pasted from ChatGPT, Claude or Copilot.

## Insert the macro
1. Edit a Confluence page.
2. Type `/Rendermark` (or open the **+** insert menu and search "Markdown, Mermaid & Code").
3. Paste your content into the editor on the left. The right side shows a live preview.
4. Click **Save**, then publish the page.

To change it later, select the macro while editing the page and click the pencil (edit) icon.

## What it renders
- **Markdown (GitHub-flavored):** headings, bold/italic, links, tables, task lists, blockquotes, inline code.
- **Mermaid diagrams:** flowchart, sequence, class, state, ER, Gantt, pie, mindmap, timeline and more. Use a fenced block:

  ````
  ```mermaid
  flowchart LR
    A --> B
  ```
  ````

  or paste a bare diagram on its own (starting with `flowchart`, `sequenceDiagram`, `graph TD`, …). It is detected automatically.
- **Code:** fenced blocks with a language (```python, ```ts, …) are highlighted; without a language, it is detected automatically.

## Diagram errors
If a diagram has a syntax error, the macro shows the parser message with the line number instead of a blank space. Fix the line in the editor and save.

## Export
PDF and Word export include the content as native Confluence text, tables and code blocks. Diagrams currently export as their Mermaid source.

## Theme
Light and dark mode follow your Confluence theme automatically.

## Security and privacy
HTML is sanitized and scripts are stripped. Mermaid runs in strict mode. The app requests no API scopes, has no backend of its own and sends no data anywhere: it runs entirely on Atlassian Forge. See the [privacy policy](rendermark-privacy.html).

## Support
Email rendermark.support@gmail.com.
