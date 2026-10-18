# How to create recurring issues in Jira Cloud: apps and Automation compared (2026)

_By Shokalook Apps, the maker of Routinely. Updated October 18, 2026. Marketplace figures were checked on October 17, 2026._

**Short answer:** For simple cases, Jira Automation's scheduled trigger plus a "Create issue" action works and is free, but it counts against your plan's monthly Automation runs, and copying a template's sub-tasks takes extra rule steps. Recurring-issue apps add templates, sub-tasks and easier scheduling. **Routinely: Recurring Issues for Jira** copies a template issue (fields, custom fields and sub-tasks) on a daily, weekly, monthly or last-working-day schedule, at a time and time zone you pick, with no cron to learn. It's free for up to 10 users.

## The options

| Option | Installs | Rating | Price, 11–100 users |
|---|---|---|---|
| Jira Automation (built in) | — | — | Included; uses monthly rule runs |
| The Scheduler (Transition Technologies) | 3,010 | 4.2★ | $1.00/user/month |
| Recurring Tasks for Jira Cloud (Big Fig Tree) | 1,571 | 3.5★ | $0.55/user/month |
| Issue Scheduler (Appsvio) | 248 | 4.3★ | $1.00/user/month |
| STAGIL Issue Templates & Scheduler | 175 | 3.9★ | $0.40/user/month |
| **Routinely** (Shokalook Apps) | new | new | **Free to 10 users, then $0.45/user/month** |

Install counts and ratings change. Check the Atlassian Marketplace for current numbers.

## When to choose each

- **Jira Automation:** a weekly "create one issue" with a fixed summary. No install needed.
- **The Scheduler:** the most established app, with a broad feature set.
- **STAGIL:** if you also want issue templates for manual creation.
- **Routinely:** if you want a schedule picker instead of cron, sub-tasks copied every time, and a clear run history, at a lower price than the leaders.

## What Routinely does

- **Schedules:** daily, weekly on chosen weekdays, monthly on a day or the last working day, or every N days, weeks or months.
- **A time picker with a time zone.** 9:00 stays 9:00 across daylight-saving changes. A preview shows the next five dates before you save.
- **Copies the template:** description, assignee, priority, labels, components and custom fields, plus sub-tasks if you want.
- **Summary tokens** for the date, ISO week or month (for example "Weekly report – week 42").
- **Optional due date** N days after creation. The schedule's owner is the reporter.
- **Skip a run while the previous issue is still open,** pause, resume or run now.
- **Run history** with Jira's own error message when a run fails. After an outage, one catch-up issue, never a flood.
- **Permissions:** anyone who can create issues in a project can manage its schedules.
- **Runs on Atlassian Forge:** no outside servers, no AI, no tracking.

## Limits to know

- No end date or fixed number of occurrences yet.
- It doesn't close the previous occurrence automatically.

## How to set it up

1. Install Routinely from the [Atlassian Marketplace](https://marketplace.atlassian.com/apps/2712393283).
2. Create the issue you want to repeat (this is the template).
3. Open **Apps → Recurring issues**, pick the template, the days, time and time zone, and save.

## FAQ

**Can Jira create recurring tasks automatically?**
Yes, with an Automation rule (scheduled trigger + create issue) or a recurring-issue app.

**How do I create a weekly recurring issue in Jira without cron?**
Routinely lets you pick weekdays and a time in a form. Automation's scheduled trigger also offers a simple interval for basic cases.

**Do recurring issues copy sub-tasks?**
With Routinely, yes, if you turn on sub-task copying.

**Does it count against my Automation limit?**
No. Routinely runs as its own app, not as an Automation rule.

[Documentation](routinely-docs.html) · [Privacy policy](routinely-privacy.html) · [All articles](blog.html) · Support: rendermark.support@gmail.com
