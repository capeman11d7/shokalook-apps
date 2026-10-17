# Answerloop: Q&A for Confluence, Documentation

Community questions and answers inside Confluence Cloud. Support: rendermark.support@gmail.com

## Getting started
1. Install Answerloop from the Atlassian Marketplace. No setup is needed: the database is created on first use.
2. Open it from the Confluence top bar: **Apps → Questions**.
3. Click **Ask a question**, pick a space, write a title and details, and add up to 5 tags.

## Asking and answering
- **Markdown** works in questions and answers: headings, lists, links, tables, `inline code` and fenced code blocks. HTML is sanitized.
- **Vote** with ▲ and ▼ on other people's posts (one vote per person; click again to clear it). You can't vote on your own posts.
- **Accept** the answer that solved it: the asker (or an admin) clicks **Accept**. The accepted answer is pinned at the top and marked ✔.
- **Edit or delete** your own posts. Deleting asks for a second click to confirm.
- **Close** a question to stop new answers (Confluence admins only). **Reopen** undoes it.

## Finding answers
- The search box matches question titles, question text and answer text, ignoring case.
- Filter by **space**, by **Unanswered**, or click a **tag** (click it again to clear it).
- The line next to the title shows how many questions there are and what share has at least one answer.
- 25 questions show at a time. Click **Load more** at the bottom for the next 25.

## The "Q&A: Questions list" macro
Put questions on any page, for example the latest onboarding questions on a new-starter page.
1. In the page editor, type `/Q&A` and insert **Q&A: Questions list**.
2. In the macro settings, enter a tag (or leave it empty for all questions) and how many to show (1–50).
3. Readers see only questions from spaces they can view. Clicking a question opens it on the Questions page.

## Permissions
- Every question belongs to a Confluence space. People see and post only in spaces they can view, so a question in a restricted space stays hidden from people outside it.
- Authors can edit and delete their own posts.
- Confluence admins (people who can administer the site) can edit, delete, close and import anything.
- Space permission changes can take up to a minute to apply.

## Importing from Questions for Confluence
Questions for Confluence **Cloud** has no export or API, so import works from a **Server or Data Center** instance (before or after you migrate).
1. On the Server/Data Center site, open `/rest/questions/1.0/question?limit=1000` while signed in and save the result as a `.json` file. For more than 1,000 questions, also save `&start=1000`, `&start=2000`, and so on.
2. If answers are not embedded in that output, also save `/rest/questions/1.0/answer/{id}` responses. One JSON array of them is fine.
3. In Answerloop, a Confluence admin clicks **Import**, picks a fallback space, then selects the files (or pastes the JSON) and clicks **Import**.

What is kept: titles, bodies, topics (as tags), accepted answers, dates and author names. Imported authors appear as names only. Questions whose space key doesn't exist on this site go to the fallback space. Running the same import again is safe: items that were already imported are skipped.

## Limits
- Up to 5 tags per question, titles up to 300 characters, bodies up to 50,000 characters.
- The tag cloud counts tags on the newest 2,000 questions. Up to 1,000 visible spaces per person are used for filtering.

## Privacy and data
All data stays in Atlassian's Forge storage for your site. The App calls no outside services and has no analytics. See the privacy policy for details.

## FAQ
**I can't find a question someone linked.** It's in a space you can't view. Ask a space admin for access.
**Why is there no Import button?** Only Confluence admins can import.
**The app says its license is inactive.** Ask a Confluence admin to renew or start a trial in **Manage apps**.
