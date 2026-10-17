# Remindly: Issue Reminders for Jira, Privacy Policy

_Last updated: October 16, 2026_

**Who we are.** Remindly: Issue Reminders for Jira ("the App") is provided by Nathan Shokalook ("we", "us"). Contact: rendermark.support@gmail.com.

## What the App does
The App is a Jira Cloud app that runs on Atlassian Forge. It lets people set reminders on Jira issues and has Jira email the chosen recipients at the chosen time.

## Data the App stores
| Data | Why | Where and how long |
|---|---|---|
| Reminder details: issue ID and key, a copy of the issue summary, the note you write, the time, time zone and repeat rule | To send the reminder and show it in the App | Forge storage, hosted by Atlassian in your site's region. Deleted 90 days after the reminder is sent or cancelled. |
| Atlassian account IDs of the person who set the reminder and of named recipients | To know who set it and who to email | Same as above. We store account IDs only, never names or email addresses (names are looked up live from Jira). |
| App settings (who may remind others, time format) | Admin configuration | Forge storage until the App is uninstalled |
| A project property marking projects where an admin turned the App off | To hide the panel there | Stored by Jira on the project |

## How reminders are delivered
The App calls Jira's own notification API, so Jira sends the email. Jira only emails people who can see the issue. The App never sees email addresses.

## Permissions the App requests
- **read:jira-work**: read the issue summary and project when you set a reminder, check admin rights, and list projects on the admin page.
- **read:jira-user**: search people and groups in the reminder form and show names.
- **send:notification:jira**: have Jira email reminders.
- **write:project.property:jira**: turn the App off per project.
- **storage:app**: store reminders and settings.

## What the App does **not** do
- We run no servers. The App runs entirely on Atlassian Forge, and no data leaves Atlassian.
- No analytics, tracking, cookies or advertising.
- We never see, collect, sell or share your content or personal data.

## Personal data reporting
Once a week the App reports the account IDs it stores to Atlassian's personal data reporting API. If an account has been closed, the App deletes the reminders that person set and removes them from other reminders.

## Third parties
**Atlassian** hosts and runs the App and stores its data. See https://www.atlassian.com/legal/privacy-policy

## Retention and deletion
Sent and cancelled reminders are deleted automatically after 90 days. Uninstalling the App removes its stored data according to Atlassian's Forge data retention.

## Your rights
For questions or deletion requests, email rendermark.support@gmail.com. We reply within 30 days.

## Changes
We will post updates here and change the "Last updated" date.
