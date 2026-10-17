# Rendermark: Rich Text & Markdown Gadget for Jira

Put announcements, sprint goals, runbooks, checklists and status notes on any Jira dashboard. They follow Jira's look, including dark mode.

## Add the gadget
1. Open a dashboard you can edit and choose **Edit** (or **Add gadget**).
2. Search for **Rich Text & Markdown** and add it.
3. Write or paste your content. The preview on the right shows exactly what viewers will see.
4. Optionally type a **title**. It replaces the gadget's default heading on the dashboard.
5. Click **Save** (or press **Ctrl+Enter** / **⌘+Enter**).

To change it later, open the gadget's menu (**⋯**) and choose **Edit**.

## What you can write
| You type | You get |
|---|---|
| `## Sprint goals` | A heading (`#` to `####`) |
| `**bold**`, `*italic*`, `~~strike~~`, `` `code` `` | Text styles |
| `[Board](https://your-site.atlassian.net/jira/boards/1)` | A link. Links to your Jira site open in the same tab, others in a new tab. `/browse/ABC-123` works too. |
| `- item` or `1. item` | Bulleted or numbered lists |
| `- [x] done` / `- [ ] to do` | A checklist |
| `\| A \| B \|` rows with a `\|---\|---\|` line | A table |
| ```` ```python ```` … ```` ``` ```` | A code block with syntax highlighting (about 35 languages) |
| ```` ```mermaid ```` … ```` ``` ```` | A diagram: flowchart, sequence, Gantt, pie and more ([Mermaid syntax](https://mermaid.js.org/intro/)) |
| `> quoted text` | A quote |
| `---` | A divider line |

Not sure of the syntax? The **Insert…** menu in the editor adds a panel, table, checklist, link, code block or diagram at the cursor.

### Callout panels
Start a quote with a marker. Text on the same line becomes the panel's title:

```
> [!WARNING] Code freeze Thursday 17:00
> Merge release branches by Thursday noon.
```

| Marker | Color |
|---|---|
| `[!INFO]` or `[!NOTE]` | Blue (information) |
| `[!SUCCESS]` or `[!TIP]` | Green (success) |
| `[!WARNING]` | Yellow (warning) |
| `[!ERROR]`, `[!CAUTION]` or `[!DANGER]` | Red (error) |
| `[!IMPORTANT]` | Purple (discovery) |

Markers are not case-sensitive. An unknown marker shows as a normal quote.

### HTML
Basic HTML works too. It is sanitized: scripts, event handlers and other unsafe markup are removed.

## Light and dark mode
The gadget follows Jira's theme (Profile → **Theme**) and switches with it. Panels, tables, code colors and diagrams all have dark variants.

## Who can edit
Only people who can edit the dashboard see **Edit** on the gadget, and Jira checks that permission again when the gadget is saved. Everyone who can view the dashboard can read the gadget.

## Limits
- Up to 30,000 characters per gadget. The editor warns you before you reach it. Use several gadgets for longer content.
- Images are shown by link only (`![alt](https://…)`). Uploading isn't supported.
- The diagram library (about 5 MB) loads only when a gadget contains a diagram, and the browser caches it after that.

## Privacy and data
Content is stored by Jira as the gadget's configuration on your dashboard. The app has no servers, sends nothing outside Atlassian, and does no tracking. Its only Jira permission (`write:dashboard:jira`) is used to set the gadget title when an editor saves. See the privacy policy.

## Troubleshooting
- **"This gadget is empty."** Nobody has added content yet. A dashboard editor can choose **Edit** in the gadget menu.
- **"This app's license is inactive."** Ask a Jira admin to renew the app's subscription in **Apps → Manage apps**.
- **"Diagram error: …"** The Mermaid text has a mistake. The message names the line. Fix it in the editor; the preview updates as you type.
- **"Jira refused the title"** when saving. You may have lost edit permission on the dashboard. Ask the dashboard owner.

## Support
Email rendermark.support@gmail.com.
