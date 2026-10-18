# Routinely: Recurring Issues for Jira

Pick an issue as a template, choose when it repeats, and Jira gets a fresh copy on schedule.

## Where to find it
- **In a project:** the project's sidebar → **Recurring issues** (schedules for that project only).
- **Across projects:** **Apps → Recurring issues** in Jira's top navigation (schedules in every project where you can create issues).

## Create a schedule
1. Click **New schedule**.
2. **Template issue:** type an issue key or a few words of its summary and pick it. The template must be a standard issue, not a sub-task. On a project's page it must be in that project.
3. **Summary:** what each new issue is called. It starts as the template's summary plus `{{date}}`. Tokens:
   - `{{date}}` → 2026-10-19
   - `{{week}}` → 2026-W43 (ISO week)
   - `{{month}}` → October 2026
4. **Repeat every** N day(s), week(s) or month(s):
   - **Weekly:** tick the weekdays.
   - **Monthly:** a day of the month (on the 29th–31st, shorter months use their last day), or **the last working day** (the last Monday–Friday; public holidays aren't known).
5. **Starting** date, **time** (15-minute steps) and **time zone**. It starts as your Jira profile's time zone.
6. Options:
   - **Due date N days after it's created** (0 = the same day).
   - **Copy the template's sub-tasks** under each new issue.
   - **Skip if the previous issue is still open:** no new copy while the last one isn't done.
7. Check the **Next:** preview (the next five dates), then click **Create schedule**.

## When issues are created
- Jira runs the app once an hour, so an issue appears **within an hour after** its time. Every schedule that's due is handled in the same run.
- The time is wall-clock time in the schedule's time zone: 9:00 stays 9:00 when daylight saving starts or ends. A time that doesn't exist on the change day (such as 02:30) runs an hour later that day.
- **Missed runs:** if Jira couldn't run the app for a while, the schedule creates **one** issue for the most recent missed date, then continues normally. It never creates a backlog of copies.
- Jira can occasionally start the same hourly run twice. Each date is claimed once, so you still get one issue.

## What gets copied
- Everything on the target issue type's **create screen** that has a value in the template: description, assignee, priority, labels, components, fix versions, custom fields (including required ones), parent or epic, and original estimate.
- Not copied: attachments, links, comments, the sprint (a closed sprint would fail) and the rank.
- **Reporter:** the person who created the schedule, if Reporter is on the create screen. Otherwise Jira uses the app as the reporter.
- **Due date:** set from the schedule. If Due date isn't on the create screen, the app sets it right after creating the issue.
- The issue is created by the app ("Routinely" shows as the creator), so it works even when the owner is away.

## Manage schedules
On each schedule:
- **Run now** creates an issue immediately. It doesn't change the next scheduled date and ignores the "skip if open" option.
- **Pause / Resume.** Resuming continues from now; dates missed while paused are not created.
- **Edit** changes anything. The owner stays the same.
- **History** shows the last 10 runs: **Created** (with the issue), **Skipped** (with the reason) or **Failed** (with Jira's message). History is kept for 90 days.
- **Delete** (click twice to confirm). Issues already created stay.

## Who can do what
- Anyone with **Create issues** permission in a project can see and manage that project's schedules. People without it see a short message instead of the list.
- Saving checks that you can see the template issue.
- Scheduled issues are created by the app with the app's permissions, as the schedule's owner set them up.

## Troubleshooting
- **Failed: "… is required."** A required field is empty in the template, or isn't on the create screen. Fill it in on the template, then use **Run now** to check.
- **Failed: "Template … no longer exists."** The template was deleted or moved. Edit the schedule and pick another one.
- **Skipped: "… is still open."** The previous issue isn't done yet and "Skip if the previous issue is still open" is on.
- **Paused: "The owner's Atlassian account was closed."** Edit and save the schedule; you become the new owner and reporter.
- **Nothing happened at the time.** Give it up to an hour. If the app's license is inactive, the page shows a warning and no issues are created until a Jira admin renews it.

## Limits
- Times in 15-minute steps; issues appear within an hour after the time.
- Up to 99 between repeats (days, weeks or months).
- Only standard issues as templates (their sub-tasks can be copied).
- Service-management request types, auto-closing old copies and bulk changes aren't supported yet.

## Privacy
Routinely runs entirely on Atlassian Forge. It stores schedules and 90 days of run history, keeps account IDs but never names or emails, and sends nothing outside Atlassian. See the privacy policy.

## Support
Email rendermark.support@gmail.com. We reply within two business days.
