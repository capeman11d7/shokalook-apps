# Onlook: Who's Viewing for Jira

See who else is looking at a Jira issue right now, and who viewed it in the last 30 days.

## See who's looking
1. Open any issue. In the details area on the right, expand **Who's looking**.
2. Avatars show everyone else who has the issue open right now, with their names underneath. Hover an avatar for the name; past five people, a **+N** avatar lists the rest.
3. When someone opens the issue you're on, Jira shows a small notice: "Priya Shah is looking at this issue too". Click **Don't show these** on the notice to stop them in this browser.

Presence works even while the **Who's looking** section is collapsed, so the notices still appear. Jira may collapse the section again on your next issue; expand it whenever you want the full list.

## How quickly it updates
- Someone who opens the issue appears within a second or two.
- Someone who closes the tab or moves to another issue disappears within about a minute.
- Switching to another browser tab or minimizing the window counts as leaving. Coming back counts as joining again.
- Your own other tabs on the same issue aren't shown as other people. The panel just notes "You also have this issue open in another tab."

## Recently viewed
Click **Recently viewed** in the panel to see the last 10 people who viewed the issue, newest first, with how long ago. A view counts after about 10 seconds on the issue, at most once every 30 minutes per person. Views are kept for 30 days. People who can no longer see the issue are left out.

## For Jira admins
Go to **Jira settings (⚙) → Apps → Onlook**:
- **Show presence:** on in every project unless you turn it off. In a turned-off project, the panel is hidden and nothing is shared or recorded.
- **Names visible to:** **Everyone**, or **Admins only** (Jira admins and that project's admins). With Admins only, everyone else sees "3 other people are looking" and a count in Recently viewed, without names.
- Use **Filter projects** to find a project. The list shows 50 at a time.

## Limits
- Live presence needs the issue open in a visible browser tab. It hasn't been tested in Jira's mobile apps.
- Up to five avatars are shown, plus a **+N** for the rest. Recently viewed shows 10 people.
- Very busy sites: Atlassian limits live presence traffic to 50 messages per second per site. Under that limit, viewers on a site with several thousand people on issues at once may show up a little late.
- No editing-conflict warnings. Onlook shows who is there, not what they are typing.

## Troubleshooting
- **I don't see the Who's looking section.** An admin may have turned presence off for this project. On a small window, scroll down the details area.
- **Someone is listed who already left.** They drop off within about a minute. If their browser crashed, it can take up to a minute too.
- **I see a count but no names.** The project is set to show names to admins only.
- **"This app's license is inactive."** Ask a Jira admin to renew the subscription.

## Privacy
Onlook runs entirely on Atlassian Forge. It stores account IDs for Recently viewed (30 days), never names or emails, and sends nothing outside Atlassian. See the privacy policy.

## Support
Email rendermark.support@gmail.com. We reply within two business days.
