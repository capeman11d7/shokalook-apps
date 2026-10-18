# Routinely: Recurring Issues for Jira, Privacy Policy

_Last updated: October 17, 2026_

**Who we are.** Routinely: Recurring Issues for Jira ("the App") is provided by Nathan Shokalook ("we", "us"). Contact: rendermark.support@gmail.com.

## What the App does
The App is a Jira Cloud app that runs on Atlassian Forge. It creates Jira issues on a schedule by copying a template issue that you choose.

## Data the App stores
| Data | Why | Where and how long |
|---|---|---|
| Schedule settings: project ID and key, template issue key, summary pattern, repeat rule, time, time zone, start date and options | To create issues on time | Forge storage, hosted by Atlassian in your site's region, until the schedule is deleted or the App is uninstalled |
| The Atlassian account ID of the person who owns the schedule | To set them as the reporter of each new issue | Same as above. We store the account ID only, never names or email addresses (names are looked up live from Jira) |
| Run history: when each run happened, its result, the key of the issue it created and any error message from Jira | To show what happened and why a run failed | Forge storage. Deleted automatically after 90 days |
| The key of the most recent issue a schedule created | For the "skip if the previous issue is still open" option | With the schedule |

The App does not copy issue content into its own storage. Field values are read from the template issue and written straight into the new issue in your Jira site.

## Permissions the App requests
- **read:jira-work**: read the template issue and its create screen, check that you may create issues in the project, and search for issues in the template picker.
- **write:jira-work**: create the scheduled issues and their sub-tasks, and set a due date.
- **read:jira-user**: show the schedule owner's name.
- **storage:app**: store schedules and run history.
- **report:personal-data**: report the stored account IDs to Atlassian, as Atlassian requires.

## What the App does **not** do
- We run no servers. The App runs entirely on Atlassian Forge, and no data leaves Atlassian.
- No analytics, tracking, cookies, advertising or AI.
- We never see, collect, sell or share your content or personal data.

## Personal data reporting
Once a week the App reports the account IDs it stores to Atlassian's personal data reporting API. If an account has been closed, the App removes that account ID from its schedules and pauses them until someone else takes them over.

## Third parties
**Atlassian** hosts and runs the App and stores its data. See https://www.atlassian.com/legal/privacy-policy

## Retention and deletion
Run history is deleted automatically after 90 days. Deleting a schedule removes it at once. Uninstalling the App removes its stored data according to Atlassian's Forge data retention. Issues the App created stay in Jira like any other issue.

## Your rights
For questions or deletion requests, email rendermark.support@gmail.com. We reply within 30 days.

## Changes
We will post updates here and change the "Last updated" date.
