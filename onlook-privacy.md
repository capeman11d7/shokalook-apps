# Onlook: Who's Viewing for Jira, Privacy Policy

_Last updated: October 17, 2026_

**Who we are.** Onlook: Who's Viewing for Jira ("the App") is provided by Nathan Shokalook ("we", "us"). Contact: rendermark.support@gmail.com.

## What the App does
The App is a Jira Cloud app that runs on Atlassian Forge. It shows who else is viewing a Jira issue right now, and who viewed it recently.

## Data the App handles
| Data | Why | Where and how long |
|---|---|---|
| Live presence messages: your Atlassian account ID and a random ID for the browser tab, sent while you have an issue open | To show other viewers of the same issue that you're there | Sent through Atlassian's Forge Realtime service to other people who have the same issue open. Not stored by the App. Each message is only delivered to people who can view that issue. |
| Recently viewed: your Atlassian account ID, the issue ID and the time you viewed it | To show the last 10 viewers of an issue | Forge storage, hosted by Atlassian in your site's region. Each entry is deleted automatically after 30 days. |
| A project property with the project's settings (presence off, or names for admins only) | Admin configuration | Stored by Jira on the project |

We store account IDs only, never names, email addresses or avatars. Names are looked up live from Jira by the person viewing, with Jira's own profile-visibility rules.

## Who can see what
- Only people who can view an issue can see who is looking at it or who viewed it recently. "Recently viewed" re-checks each person's access to the issue every time it is shown, so someone who lost access is not listed.
- Jira admins can turn the App off per project, or show names only to Jira admins and project admins. Everyone else then sees a count instead of names.
- A per-person "Don't show these" option turns off the pop-up notices in that browser.

## Permissions the App requests
- **read:jira-work**: read project settings and check admin rights.
- **read:jira-user**: show viewers' names and check that a viewer can still see the issue.
- **write:project.property:jira**: save per-project settings from the admin page.
- **storage:app**: keep the recently viewed list.

## What the App does **not** do
- We run no servers. The App runs entirely on Atlassian Forge, and no data leaves Atlassian.
- No analytics, tracking, cookies or advertising. The browser's local storage holds only two conveniences: which issues you viewed in the last 30 minutes (so a view isn't recorded twice) and the "Don't show these" choice.
- We never see, collect, sell or share your content or personal data.

## Personal data reporting
Once a week the App reports the account IDs it stores to Atlassian's personal data reporting API. If an account has been closed, the App deletes that person's entries.

## Third parties
**Atlassian** hosts and runs the App, delivers the live presence messages, and stores its data. See https://www.atlassian.com/legal/privacy-policy

## Retention and deletion
Recently viewed entries are deleted automatically after 30 days. Live presence messages are not stored by the App. Uninstalling the App removes its stored data according to Atlassian's Forge data retention.

## Your rights
For questions or deletion requests, email rendermark.support@gmail.com. We reply within 30 days.

## Changes
We will post updates here and change the "Last updated" date.
