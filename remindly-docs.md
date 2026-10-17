# Remindly: Issue Reminders for Jira

Set reminders on Jira issues for yourself or your team. Jira emails the recipients when a reminder is due.

## Set a reminder
1. Open an issue. In the **Reminders** panel, click **Set reminder**. (In Jira's issue view, apps' panels may sit behind the **Apps** button the first time you use them.)
2. Pick a time: use a quick pick (**In 1 hour**, **Tomorrow 9:00**, **Next Monday 9:00**) or choose a date and a time in 15-minute steps. The time zone starts as your Jira profile's; change it if the reminder belongs to another office.
3. Choose who to remind: **Me**, **Assignee**, **Reporter**, and/or search for people and groups.
4. Optionally add a note (up to 500 characters) and a repeat: every day, week or month.
5. Click **Set reminder**.

Reminders go out within 5 minutes of their time.

## What recipients get
- A Jira email with your note and a link to the issue. If someone else set it, the email says who.
- Named people (and you, for your own reminders) also see a banner on the issue for 24 hours after it goes off.
- Jira only emails people who can see the issue. Assignee and reporter mean whoever holds that role when the reminder goes off.

## Repeating reminders
- **Every day / week:** same wall-clock time, even across daylight-saving changes.
- **Every month:** same day of the month; on the 29th–31st it uses the last day of shorter months.
- If Jira was unreachable for a while, a missed occurrence is sent once, not replayed.
- Each sent occurrence appears in **History**. Cancelling stops the whole series.

## Snooze, edit and cancel
On the issue panel or the **Reminders** page (**Apps → Reminders**):
- **Snooze…** moves the next send by 15 minutes, 1 hour, or to tomorrow 9:00. Snoozing a reminder that already went off sets it again, once.
- **Edit** changes the time, recipients, note or repeat of an upcoming reminder.
- **Cancel reminder** (click twice to confirm) stops it.

The **Reminders** page has three tabs: **Upcoming** (your reminders for yourself), **Set for others**, and **History** (sent, failed and cancelled, kept for 90 days). Reminders other people set for you show on the issue itself.

## For Jira admins
Go to **Jira settings (⚙) → Apps → Reminders** in the sidebar:
- **Who can set reminders for other people:** everyone, Jira admins only, or nobody (everyone can still remind themselves). This is enforced by the app, not just hidden in the form.
- **Time format:** each user's language, 12-hour, or 24-hour.
- **Projects:** Reminders are on in every project unless you turn a project off. A turned-off project doesn't show the panel; reminders already set there still go out.

## Limits
- Up to 20 people and 5 groups per reminder. Notes up to 500 characters.
- Times in 15-minute steps; delivery within 5 minutes of the time.
- History is kept for 90 days.
- Reminders arrive by email only. Slack, Teams and mobile push aren't supported.

## Troubleshooting
- **No email arrived.** Check the recipient can view the issue, and look in spam. Jira sends from its usual notification address. A reminder that couldn't be sent shows as **Failed** in History with the reason.
- **"Your Jira admin only allows reminders for yourself."** An admin restricted reminders for others. Ask them.
- **"You can't see this issue."** You need permission to view the issue to set a reminder on it.
- **No Reminders panel.** An admin may have turned the project off, or open the panel from the issue's **Apps** button.
- **"This app's license is inactive."** Reminders aren't sent until a Jira admin renews the subscription.

## Privacy
Remindly runs entirely on Atlassian Forge, stores account IDs but never names or emails, deletes history after 90 days, and sends nothing outside Atlassian. See the privacy policy.

## Support
Email rendermark.support@gmail.com. We reply within two business days.
