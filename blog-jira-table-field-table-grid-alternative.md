# How to add a table field to Jira issues: Table Grid alternatives compared (2026)

_By Shokalook Apps, the maker of Rowsmith. Updated October 18, 2026. Marketplace figures were checked on October 16, 2026._

**Short answer:** Jira Cloud has no built-in table custom field, so line items, test steps, parts lists or approvals need an app. The leading app, Table Grid Next Generation, is rated 3.5★, and its most common complaint is that grids can't be filled in on the create-issue screen. **Rowsmith: Table Field for Jira** is a real Jira custom field: it works on the create screen, transitions, the issue view, the customer portal and bulk edit, with typed columns, totals, paste from Excel and CSV export. It's free for up to 10 users and about 30% cheaper than Table Grid above that.

## The options

| App | Installs | Rating | Price, 11–100 users |
|---|---|---|---|
| Table Grid Next Generation (Exalate) | 1,158 | 3.5★ | about $0.73/user/month ($8.70/user/year) |
| Excel-like Tables for Jira | 346 | 4.0★ | see listing |
| Quick Tables for Jira | 79 | — | see listing |
| Kepler SQL Query Fields | 78 | — | see listing |
| **Rowsmith** (Shokalook Apps) | new | new | **Free to 10 users, then $0.50/user/month** |

Install counts and ratings change. Check the Atlassian Marketplace for current numbers.

## When to choose each

- **Table Grid Next Generation:** the most established option, with advanced grid features and a long history.
- **Excel-like Tables:** if you want spreadsheet-style editing and import.
- **Kepler:** if your table should be filled from a SQL query rather than typed in.
- **Rowsmith:** if people must fill the table **when they create the issue** or during a workflow transition, or you need it in the customer portal or bulk edit.

## What Rowsmith does

- **A real custom field** (Forge `jira:customField`), so you place it on screens like any other field: create, transition, issue view, portal request and bulk edit.
- **Typed columns,** up to 10 per field: text, number, date, select, user, checkbox and link. Required columns are checked before saving.
- **Paste rows from Excel or Google Sheets,** reorder and delete rows, and see totals for number columns.
- **CSV download** for any table, and issue exports include a short summary of each table.
- **As many Table fields as you need,** each with its own columns.
- **Runs on Atlassian:** the values are stored as Jira field data. No outside servers, no AI.

## Limits to know

- Up to 100 rows and about 32,000 characters per table (Jira's field limit).
- JQL can search a table's text (`Field ~ "word"`) but can't filter on one column.
- Jira Automation sees the table as one JSON value.

## How to set it up

1. Install Rowsmith from the [Atlassian Marketplace](https://marketplace.atlassian.com/apps/2429925044).
2. In Jira settings, create a custom field of type **Table** and define its columns in the field context.
3. Add the field to your create and edit screens.

## FAQ

**Can Jira Cloud have a table custom field?**
Not natively. An app like Rowsmith or Table Grid adds one.

**How do I add line items to a Jira issue?**
Create a Table field with columns such as Item, Quantity and Price. Rowsmith totals the number columns automatically.

**Can people fill the table on the create-issue screen?**
With Rowsmith, yes. It's a native custom field, so it appears on create, transition and portal screens.

**Can I paste from Excel?**
Yes. Copy cells in Excel or Google Sheets and paste them into the table editor.

[Documentation](rowsmith-docs.html) · [Privacy policy](rowsmith-privacy.html) · [All articles](blog.html) · Support: rendermark.support@gmail.com
