# Rowsmith: Table Field for Jira, Documentation

Rowsmith adds a **Table** custom field type to Jira Cloud. Each Table field has its own columns, and each issue holds up to 100 rows.

## 1. Create a Table field (Jira admin)
1. Go to **Settings → Issues → Custom fields → Create custom field**.
2. Pick **Table** (from Rowsmith), give it a name such as "Line items", and add it to the screens you want: create, edit, view and transition screens.
3. Open the field's **Contexts and default value**, choose a context, and open the **Rowsmith column settings**.
4. Add up to 10 columns. For each one, choose a name, a type and whether it's required. Select columns need a comma-separated list of options.
5. Click **Save**.

Need different columns for different projects? Create another context with its own columns, or create another Table field.

### Column types
| Type | Stores | Notes |
|---|---|---|
| Text | Any text, up to 1,000 characters per cell | |
| Number | A number | Shown with a totals row. Pasted values like `1,234.50` or `$12` are understood |
| Date | A day (YYYY-MM-DD) | Uses your browser's date picker |
| Select | One of the options you defined | Pasted values match options ignoring case |
| User | A Jira person | Type 2+ letters to search. Pasted names are kept as text |
| Checkbox | Yes/No | A required checkbox must be ticked |
| Link | An http(s) URL | Opens in a new tab |

Renaming a column keeps its data, because rows store a hidden column id. Deleting a column hides it from the editor, but issues that already have data in it still show that column until the rows are edited.

## 2. Fill in a table
The table appears wherever the field is on a screen: **create issue**, the **issue view**, **transition screens**, the **customer portal** request form, and **bulk edit**.
- **+ Add row** adds a row. ↑ and ↓ reorder rows, and ✕ deletes one.
- **Paste from Excel or Google Sheets:** copy a block of cells, click the cell where it should start, and paste. If the first pasted line matches the column names, it's skipped as a header. Rows past 100, or cells past the last column, are dropped with a notice.
- Required columns and invalid values (for example text in a Number column) are highlighted, and **Save** stays blocked until they're fixed.
- Empty rows are dropped when you save.
- On the issue view, use the table's **Save** or **Cancel**. On create, transition, portal and bulk edit there's no separate Save: valid changes go into the form as you type ("Saved to the form"), and Jira's own Create / Update button saves them.

## 3. Read and export
- The issue view shows the table read-only, as a native Jira table with a totals row. Click it to edit (if you have edit permission). In the Details side panel, Jira shows the short summary instead; move the field to the main area in the project's issue layout to show the full table there.
- **Download CSV** (in the editor) saves the table exactly as shown (UTF-8 with a header row). Cells starting with `=`, `+`, `-` or `@` get a leading `'` so spreadsheets don't run them as formulas.
- In issue lists, notifications and Jira's CSV export of search results, the field shows a short summary: the row count and the first row.

## 4. Limits
- Up to **10 columns** and **100 rows** per table.
- **JQL:** `"Line items" ~ "monitor"` finds issues whose table contains the word. You can't filter by one column (for example "Qty > 5").
- **Automation:** smart values see the whole table as one JSON value (`{"rows": [...], "summary": "..."}`), keyed by hidden column ids. The `summary` text is the easiest part to use in rules.
- The field type can't be changed after it's created (a Jira rule for all custom fields).
- If the app is uninstalled, Jira keeps the field data for 30 days, and reinstalling within that time restores it.

## Support
Email rendermark.support@gmail.com. We reply within two business days.
